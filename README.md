# ckeditor4-fix-widget-dnd

This is a Drupal-optimized build of CKEditor 4.15 which includes a fix for https://github.com/ckeditor/ckeditor4/issues/3926.

To re-create this build:
* Clone the development repo of CKEditor (https://github.com/ckeditor/ckeditor4).
* Check out the version you'd like to build.
* Apply fix-widget-dnd.patch from this repo.
* Copy build-config.js from this repo to ./dev/builder/
* Run ./dev/builder/build.sh -s
* This will create a Drupal optimised version of ckeditor in /dev/builder/releases that can replace Drupal 8's core/assets/vendor/ckeditor.

# Using the pre-build image

* Copy the contents of `build/ckeditor` to replace Drupal 8's `core/assets/vendor/ckeditor` directory.
* Clear caches.