# README.md [WIP]

## Migration to Hugo static site

Main motivation for the move:

 - dated style
 - HTML based is hard do maintain
 - unclean structure 
 - not easily compatible with different devices/browsers
 - not flexible for adding material
 - unsafe ftp hosting

Benefits for the new setup:
 - using static site generator
 - super fast and clean
 - style easy to modernise with hugo templates 
 - easily configurable via central config file
 - clean structure in hugo
 - easily customisable templates & layouts
 - modular entries (posts, gallery etc)
 - managed in its own git repository
 - easy to modify, with version control 
 - makes hosting secure and flexible
 - development and test of new features in separate branches
 - easier handover and permissions handling
 

## Migration checklist

- [x] adapt css style
- [ ] add language support (EN/EL)
- [ ] strip & migrate HTML pages (see table below)
- [ ] choose categories, menu items, etc.
- [x] create members records and feed them into members landing
- [x] create news records and feed them into news landing
- [ ] check hyperlinks
- [ ] create archetypes
- [x] setup hosting and deployment with github pages
- [ ] **important** locate source of payments.hsrgc.gr and migrate
- [ ] create members database in json file and feed that into members (optional)
- [ ] create gallery of images and showcase from home
- [ ] test draft website
- [ ] take new website live
- [ ] choose template (hsrgc custom/ananke/roadster)
- [ ] customize and final touches with template


| old URL                      | new Hugo path      | redirect needed | migration status   |
|------------------------------|--------------------|-----------------|--------------------|
| index.html                   | /_index.md         | :x:             | :construction:     |
| history.html                 | /history.md        | :x:             | :white_check_mark: |
| organization.html            | /organization/     | :x:             | :white_check_mark: |
| activities.html              | /activities/       | :?:             | :construction:     |
| membership.html              | /membership/       | yes             | :construction:     |
| members.html                 | /members/_index.md | :?:             | :construction:     |
| members/                     | /members/          | :x:             | :construction:     |
| members-2014.html            |                    |                 | will not migrate   |
| organizations.html           | /organizations/    |                 | :construction:     |
| links.html                   | /links/            |                 | :construction:     |
| public-outreach.html         | /outreach/         |                 | pending            |
| public-outreach-old.html     |                    |                 | will not migrate   |
| public-outreach-old2.html    |                    |                 | will not migrate   |
| contact.html                 | /contact.md        |                 | :construction:     |
| payments?                    |                    |                 | update needed      |
| forum?                       |                    |                 | ?                  |
| colloquia.html               | /events/           |                 | pending            |
| dntest.html                  |                    |                 | will not migrate   |
| elections-2014.html          |                    |                 | :construction:     |
| elections-2014-ann.html      |                    |                 | :construction:     |
| elections-2016.html          |                    |                 | :construction:     |
| elections-2016-results.html  |                    |                 | :construction:     |
| elections-2018-ann.html      |                    |                 | :construction:     |
| elections-2018-results.html  |                    |                 | :construction:     |
| elections-2020-ann.html      |                    |                 | :construction:     |
| elections-2022-ann.html      |                    |                 | :construction:     |
| elections-2025-results.html  |                    |                 | :construction:     |
| gr100-athens.html            |                    |                 | :construction:     |
| kip_thorne.html              |                    |                 | :construction:     |
| kip_thorne_back.html         |                    |                 | will not migrate   |
| neb19.html                   |                    |                 | will not migrate   |
| neb19-hotels.html            |                    |                 | will not migrate   |
| oup.html                     |                    |                 | update needed      |
| psaltis_auth.html            |                    |                 | :construction:     |
| test_page.html               |                    |                 | will not migrate   |
| neb17/                       |                    |                 | will not migrate   |
| neb18/                       |                    |                 | will not migrate   |
| pdf/Outreach/gr100-athens    |                    |                 | ?                  |
| pdf/Outreach/public-outreach |                    |                 | ?                  |
| pdf/Colloquia/               |                    |                 | pending            |
| pdf/Outreach                 |                    |                 | pending            |
| pdf/                         |                    |                 | pending            |



