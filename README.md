# Catalog Manager

A Single Page App (SPA) website complete front-end and back-end based on Flask and SQLAlchemy for cataloging stuff.

The website allows any logged in user to add categories and add sub-items under these categories and also edit and delete categories and items.

O-Auth login using Google is supported.

## Requirements

  * Python2
  * Flask
  * SQLAlchemy
  * Redis DB Server
  * Databse server of your choice (tested for PostgreSQL)

## Usage

* For Google O-Auth to work you must:
  1. Edit `templates/app.html` and put your client id under the content of the `meta` tag wit the name `google-signin-client_id`
  2. Save your application's `client_secrets.json` beside `catalog.py`

* Copy the file `catalog_default.ini` to `catalog.ini` and update DB connect string

* Run the Redis DB Server: `nohup redis-server &`

* Run the main app file: `nohup python catalog.py &`

* Visit "http://localhost/" on browser

## Known Issues

* Pressing edit or delete category buttons will toggle the collapse of the category
* After any edit to the catalog it will collapse all categories

## Room for improvements

* Add the ability for users to change password and upload their photo
* Add the ability to add photo and description for categories and items
* Enhance the loading screen

## Contributions

I encourage you all to contribute into this simple project to make better and more usable.
