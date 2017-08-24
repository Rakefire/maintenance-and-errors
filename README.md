maintenance.rakefire.io
========================================

Maintenance and Error pages for our clients. Repo is a collection of these pages and some helper scripts to set the error/maintenance pages on Heroku apps. Much of this work is based off of [https://devcenter.heroku.com/articles/error-pages#customize-pages]


To create/update a given set of error pages, the steps are:

1) Create a subfolder in this repository (likely clone the `/strategery` folder)

2) Customize the error and maintenance pages and add the appropriate logos

3) Push your changes to the github repository

4) Run the `update-error-pages` script with the appropriate details so that Heroku knows about the new error pages (e.g. `./bin/update-error-pages HEROKU_APP_NAME FOLDER`)


### Note: Default Heroku Pages

The `/heroku` directory contains the current pages that Heroku will serve in the case of maintenance or an error. Download the latest at: https://devcenter.heroku.com/articles/error-pages#customize-pages

Alternatively, download the latest by running `./bin/update-heroku-error-pages`
