Drupal to Static
===
**[Drupal to Static](https://github.com/kkomelin/drupal_to_static) module exports Drupal 7 site content in the Markdown format ready for static site generators, such as Jekyll, Jigsaw, etc.**

## Motivation

(TBD)

## Dependencies

- [PHP Zip extension](http://php.net/manual/en/book.zip.php)
- [Optional] [Markdownify module](https://github.com/lukaswhite/Drupal-Markdownify) if you'd like to translate your content HTML into the Markdown format.

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