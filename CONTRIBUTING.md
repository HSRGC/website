# CONTRIBUTING [WIP]

Here you will find a minimal set of guidelines on how to contribute content to the website repo.
For more advanced topics, consult the [hugo documentation](https://gohugo.io/documentation/).

## Installing Hugo

Make sure you have Hugo installed on your system.
You can follow the installation instructions for macOS, Linux, Windows or BSD on the [hugo website](https://gohugo.io/installation/) 

For macOS, the easiest way is via homebrew:

```
brew install hugo
```

## Clone the git repo

Make a local clone of this git repo to your current working directory by running

```
git clone git@github.com:HSRGC/website.git
```

## Make your contribution

Before starting to edit your local clone, make sure you have pulled the most recent changes to the repository.

Make your changes locally, typically by editing files under the `content/` directory.

If you want to create a new file, e.g. under the `news` section, you can use the Hugo command like so:

`hugo new content/news/great-news-everyone.md`

This creates the new file and initializes it with the appropriate template, for convenience and uniformity.

Then run

`hugo server -D`

to build the website and review locally (including draft pages).

Once you're happy with your edits, proceed with the typical git workflow: 
 - commit your changes, 
 - pull & resolve conflicts (if any) and 
 - push.

Alternatively, and only for simple changes that don't require testing, you can edit files directly through the github web interface.

Don't worry too much about breaking things. 
Git keeps the complete history of changes, so we can always roll back to an earlier working version if something goes wrong. 
Moreover, if deployment is set up via a github pages workflow, preliminary checks are made before a change gets approved for deployment to the online version. 

Never edit files inside `themes/<name>/`, these are submodules (except our own custom `hsrgc` theme) and should only be updated.

## Advanced 

### Changing themes

A broad list of Hugo themes can be found [here](https://themes.gohugo.io).

A new theme can be installed by adding a git submodule that clones its repo under the `themes/` subdirectory, like so:
```
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
```
Here I cloned the repository of the *Ananke* theme as a git submodule. 

The option that controls which theme will be used when the website is built is the `theme` option in the `hugo.toml` config file, currently set to 
```theme = 'ananke'```. 
Following this, you will probably have to tweak several configuration options, layouts and content files, in order to customize the website according to the new theme.
For details, check the theme's documentation.
