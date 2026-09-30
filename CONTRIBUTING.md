# CONTRIBUTING [WIP]

## Installing Hugo

Make sure you have Hugo installed on your system.
You can follow the installation instructions for macOS, Linux, Windows or BSD on the [hugo website](https://gohugo.io/installation/) 

For macOS, the easiest way is via homebrew:

`brew install hugo`

## Clone the git repo


## Make your contribution

`hugo server -D`

to build and review locally

Don't worry too much about breaking things. 
Git keeps the complete history of changes, so we can always roll back to an earlier working version if something goes wrong. 
Moreover, if deployment is set up via a github pages workflow, preliminary checks are made before a change gets approved for deployment to the online version. 

Never edit files inside `themes/<name>/`, these are submodules and should only be updated.

## Advanced 

### Changing themes

A broad list of Hugo themes can be found [here](https://themes.gohugo.io).

A new theme can be installed by adding a git submodule that clones its repo under the `themes/` subdirectory, like so:
```
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
```
Here I cloned the repository of the *Ananke* theme as a git submodule. 

The option that controls which theme will be used when the website is built is the `theme` option in the `hugo.toml` config file, currently set to 
```theme = 'ananke'```
