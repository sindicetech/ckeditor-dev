# CKE Editor Customized for Annotations

This repository contains a fork of the CKE editor with the "hiddenfields" 
feature customized to insert annotations.

See [Teckro - Guide to Annotating](https://docs.google.com/document/d/1K_P1F_a7sNUiVzWv_ErTT4tVGsKNLwreJYkVeZRBxGY/edit#heading=h.fnkdbgioz8kb)
and [Teckro - CMS Options](https://docs.google.com/document/d/1vLI4db2IzogyMAPWMAWDAg63sAOsoct2bEc4xqw2aUc/edit#heading=h.72i6mbrphbu9)

The customization affects mostly two files:

 - plugins/fakeobjects/plugin.js
 - plugins/forms/dialogs/hiddenfield.js

It's two files because one deals with translating the input tag into 
the annotation icon with a tooltip and the other one manages the other
direction (if I remember correctly).

# Building

Read the original readme - basically, execute `./dev/builder/build.sh`

# Integrating with Drupal

Replace the directory `/var/www/drupal/sites/all/modules/ckeditor/ckeditor` (sic)
with the result of the build above.


