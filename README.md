Drupal to Static
===
[Drupal to Static](https://github.com/kkomelin/drupal_to_static) module exports Drupal 7 site content in the Markdown format for static site generators, such as [Jekyll](https://jekyllrb.com/), [Jigsaw](http://jigsaw.tighten.co/), etc.

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

## Changes compared to [lukaswhite/Drupal-Jekyll-Export](https://github.com/lukaswhite/Drupal-Jekyll-Export)

- [x] [Added GPLv2 license file](https://github.com/kkomelin/drupal_to_static/issues/1)
- [x] [Renamed the module from `jekyll_export` to `drupal_to_static`](https://github.com/kkomelin/drupal_to_static/issues/2)
- [x] Changed configuration path to `admin/config/development/drupal_to_static`
- [x] [Used version branch `7.x-1.x` instead of `master`](https://github.com/kkomelin/drupal_to_static/issues/3)
- [x] [Removed "Include unpublished nodes?" option](https://github.com/kkomelin/drupal_to_static/issues/9)
- [x] [Made Markdownify optional](https://github.com/kkomelin/drupal_to_static/issues/7)
- [x] [Made dates in file names optional](https://github.com/kkomelin/drupal_to_static/issues/5)
- [x] [Fixed bug: File names of localized nodes are not correct](https://github.com/kkomelin/drupal_to_static/issues/10)
- [x] [Supported multilingualism](https://github.com/kkomelin/drupal_to_static/issues/8) See also [#16](https://github.com/kkomelin/drupal_to_static/issues/16)
- [x] Fixed potential bug: Improper use of strrpos() - the position of an occurrence can be 0.
- [x] Refactoring: extracted some code to separate functions.
- [x] [Implemented export of meta description from metatags module](https://github.com/kkomelin/drupal_to_static/issues/12)
- [x] [Applied Drupal's content filter to body field content before writing it to a file](https://github.com/kkomelin/drupal_to_static/issues/13)
- [x] [Added an option to skip adding language field for nodes in the default site language](https://github.com/kkomelin/drupal_to_static/issues/11) See also [#15](https://github.com/kkomelin/drupal_to_static/issues/15)
- [x] [Added support for layout fields of both Jekyll and Jigsaw](https://github.com/kkomelin/drupal_to_static/issues/14)

## Credits

Author: [Lukas White](https://github.com/lukaswhite) (hello@lukaswhite.com)  
Modified by: [Konstantin Komelin](https://github.com/kkomelin)


## License

GNU GPL v2.0 ([why?](https://github.com/kkomelin/drupal_to_static/issues/1#issue-344303013))