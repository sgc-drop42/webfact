webfact: core logic module

The Webfactory provides a UI to interface to the Docker API, allowing operations on containers/images. It aims to streamline dev and operations for Drupal websites. See also https://github.com/Boran/webfact

The Webfactory consists of several modules: webfact (main logic), webfact_content_types (features/views), webfact-make (build/install), webfactapi (optional remote control) and webfactory (deprecated)

You need:
  Docker server (e.g. Ubuntu 14.04) with docker 1.5 or later
  Container for the webfactory (e.g. the drupal lamp "boran/drupal" container)
  This module and the webfactfeature module
  Some Drupal contrib modules.
  Bootstrap theme and link in the theme function for status fields

Installation
----------------
See the readme in the webfact-make repo.


Programming notes
-----------------
See test.php cmdline.php for examples on using the apis and testing individual functions.
* Tested with Docker API v1.15
* The docker-php library (https://github.com/stage1/docker-php) 
* The guzzle http client is used. This makes porting with Drupal8 (if fact the first attempt was on Drupal 8 and then focus was shifted back to D7), hence the dependancy on the composer_manager module


