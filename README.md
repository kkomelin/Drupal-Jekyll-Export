Drupal to Static
===
**[Drupal to Static](https://github.com/kkomelin/drupal_to_static) module exports Drupal 7 site content in the Markdown format ready for static site generators, such as Jekyll, Jigsaw, etc.**

## Motivation

(TBD)

## Changes compared to [lukaswhite/Drupal-Jekyll-Export](https://github.com/lukaswhite/Drupal-Jekyll-Export)

- Added GPLv2 license file (https://github.com/kkomelin/drupal_to_static/issues/1)
- Renamed the module from `jekyll_export` to `drupal_to_static` (https://github.com/kkomelin/drupal_to_static/issues/2)
- Changed configuration path to `admin/config/development/drupal_to_static`
- Used version branch `7.x-1.x` instead of `master` (https://github.com/kkomelin/drupal_to_static/issues/3)
- Removed "Include unpublished nodes?" option (https://github.com/kkomelin/drupal_to_static/issues/9)
- Made Markdownify optional (https://github.com/kkomelin/drupal_to_static/issues/7)
- Make dates in file names optional (https://github.com/kkomelin/drupal_to_static/issues/5)

## Dependencies

- [PHP Zip extension](http://php.net/manual/en/book.zip.php)
- [Optional] [Markdownify module](https://github.com/lukaswhite/Drupal-Markdownify) if you'd like to convert your HTML content to the Markdown format.

## Installation

Copy/clone the module into your `sites/all/modules/contrib` and enable it as usual from the admin panel or through drush.

## Usage

1) Once you've installed the module, browse to `admin/config/development/drupal_to_static`

2) Select the content types to export, enter the name of the layout, and hit "Run Export".

3) Download the ZIP file which the module produces for you. 
The archive should contain all the specified nodes in Markdown format. 

4) Then copy the content of the archive into the `_posts` folder of your site generator setup.


## Credits


Author: [Lukas White](https://github.com/lukaswhite) (hello@lukaswhite.com)  
Modified by: [Konstantin Komelin](https://github.com/kkomelin)


## License

GNU GPL v2.0 ([why?](https://github.com/kkomelin/drupal_to_static/issues/1#issue-344303013))