=== GP Bulk Download Translations ===
Contributors: GregRoss
Donate link: http://toolstack.com/donate
Plugin URI: http://glot-o-matic.com/gp-bulk-download-translations
Author URI: http://toolstack.com
Tags: translation, glotpress
Requires at least: 4.4
Tested up to: 6.6
Stable tag: 1.2
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

A plugin for GlotPress as a WordPress plugin that downloads all translation sets for a project as a single zip file.

== Description ==

A plugin for [GlotPress as a WordPress plugin](https://github.com/GlotPress/GlotPress-WP) that downloads all translation sets for a project as a single zip file.

== Installation ==

Install from the WordPress plugin directory.

By default PO files will be exported, you can set which formats will be exported by adding the following line to your wp-config.php file (only include those lines for the formats you wish to export):

	define( 'GP_BULK_DOWNLOAD_TRANSLATIONS_FORMAT_PO', true );
	define( 'GP_BULK_DOWNLOAD_TRANSLATIONS_FORMAT_MO', true );
	define( 'GP_BULK_DOWNLOAD_TRANSLATIONS_FORMAT_ANDROID', true );
	define( 'GP_BULK_DOWNLOAD_TRANSLATIONS_FORMAT_RESX', true );
	define( 'GP_BULK_DOWNLOAD_TRANSLATIONS_FORMAT_STRINGS', true );

	Note: If you have custom formats defined you can use 'GP_BULK_DOWNLOAD_TRANSLATIONS_FORMAT_[SLUG]' to include them (SLUG must be in upper case and any dashes replaced with underscores).

You can also define the temporary directory to use by adding the following line to your gp-config.php file:

	define( 'GP_BULK_DOWNLOAD_TRANSLATIONS_TEMP_DIR', 'c:/temp' );

	Note: Do not include a trailing slash.

== Frequently Asked Questions ==

= TBD =

TBD

== Changelog ==
= 1.2 =
* Release date: November 11, 2024
* PHP 8.1 compatibility with not dynamically creating variables

= 1.1 =
* Release date: June 20, 2016
* Renamed main plugin file.
* Fixed gp_export_translations_filename filter passing an incorrect parameter, thanks DavidAnderson684.
* Fixed incorrect locale parameter being passed to export code.
* Updated file generation code to it's own function to allow for other plugins to use it.

= 1.0 =
* Release date: March 18, 2016
* Official 1.0 release and some minor documentation updates.

= 0.6 =
* Release date: January 15, 2016
* Fixed use of filter for file names.

= 0.5 =
* Release date: December 14, 2015
* Initial release.
