=== WP-HeadlineAnimator ===
Contributors: Viktoria Rei Bauer
Donate link: http://my.stargazer.at/wishlist/
Tags: post,image,signature
Requires at least: 2.9
Tested up to: 4.6
Stable tag: trunk


WP-Headlineanimator generates an animated GIF File to be displayed in signatures
or wherever you like to advertise for your Blog.

== Description ==
WP-Headlineanimator is a Plugin for Wordpress. It generates an animated GIF File to be displayed in signatures or wherever you like to advertise for your Blog.

= Requirements =
* Wordpress >= 2.9
* some time
* Access to your webserver
* A background picture for your signature
* A Font file (ttf)
* PHP with GDlib support

= Features =
* As a forum signature can be called _very_often_, it is pointless generating the picture from scratch via PHP
* The gif image is updated everytime you WRITE, DELETE or MODIFY a post.
* The Plugin is qTranslate-Compatible (this is a plugin for multilingual blogs)

= Languages =
* English
* German
* Turkish (thanks to MysD)

If you want to see this plugin in your language, feel free to contact me or use [transifex.net](https://www.transifex.net/projects/p/wpha/resource/plugin/) to contribute.

= Links =
* [Blog](http://my.stargazer.at/ "Authors blog")
* [Bugtracker](http://bugs.stargazer.at/ "Bugtracker")
* [Twitter](http://www.twitter.com/ToeiRei)


== Installation ==
1. Upload the contents of the wp-headlineanimator directory into your wordpress plugin directory.
2. make sure that the file you want to write your animator to is writeable for php
3. Activate the Plugin
4. Configure the Plugin via the admin interface
5. Enjoy and be so kind giving some feedback to me on my blog

== Configuration ==
 The configuration takes place in the administrative backend on
 Options -> WP-HeadlineAnimator. The options are kept to a minimum to keep it
 simple and intuitive. Basic options here:

Background image: 	This text field requires the path to your HeadlineAnimator
			Background picture relative to your WordPress installation.
			If the picture is not accessible, the label is shown in red

Font file:		This text field requires the *absolute* path to a font
			file (ttf) on your server. It is used to write text on the
			Background image. If the fomt file is not accessible,
			the label is shown in red

Target:			This is the path where your image should be written to;
			relative to your WordPress Installation

Text on Picture:	Text entered here is shown on the Animator.

Text Color: 		Enter a color here in Hex format (#ffffff is white). This
			color will be used for the text on the picture.

Show date on animator:	If you want your headlines to be prefixed with a date,
			check this box.

Date format:		This is direct access to the PHP date() function used
			to display the date prefix of your headlines.

If you got things right, "HTML Code for your Animator" is shown including your
animator.

== Frequently Asked Questions ==
= The plugin shows the StarBlog background =
Just draw your own background image, upload and use the new filename in the config

= The configuration labels of background picture and/or font file are written in red =
If the labels are written in red, the plugin cannot access the files. Keep in mind:
* the background picture path is relative to your wordpress directory
* the font file uses an absolute path as most distributions are installing fonts to /usr/share/fonts/...

= Does the remote FTP Server need to have PHP or something like that? =
The remote FTP server will just act as a file storage.

= I got a question not covered by this FAQ =
Feel free to contact me. I'll extend the FAQ with your questions and provide support.

== Bugs ==
* no error handler on if output file is not writeable


== Changelog ==

= 1.7.3 =
* Style update
* Translation fixes

= 1.7.2 =
* Style fix
* readme updates

= 1.7.1 =
* Bugfix push for getting Turkish translation published
* Add GPL Header to adminpanel
* Added Link to Bugtracker / Blog

= 1.7.0 =
* Localization
* Refresh admin interface

= 1.6 =
* Corrected PHP short-tag settings issue
* drop support for wp < 3.0

= 1.5 =
* Fixed a typo
* Changed from Polyglot to qTranslate Support

= 1.4 =
* Timing is now configureable
* Added FTP Upload option

= 1.3 =
* Font size now customizeable
* Split off administration to seperate file
* Introduced simple and advanced configuration
* Got rid of the last hardcoded path information
* Number of headlines to be displayed is now customizeable
* Seperated display of the animator in the admin panel

= 1.2 =
* Reintroduced Polyglot support as it just did some weird
* got rid of exif - caused many problems on some systems.
* added BBCode Line for copy&paste
* Textcolor is now changeable

= 1.1 =
* Ripped out Polyglot detection as this is already handled by wordpress with get_posts()
* Added initialisation routine for default options
* Preview only if file exists
* Only write file if we got a font and picture

= 1.0 =
* Let's assume I got my wishlist completed on that topic and the code isn't too ugly.

= 0.6 =
* Got rid of tmp path; we just write out our image
* cleanup
* picture format support

= 0.5 =
* Upgrade to new GifMerge Class
* eliminating of direct DB Queries
* code cleanups

= 0.4 =
* make use of polyglot_filter() for better Polyglot Support -> Multilanguage!!
* minior design fixes

= 0.3 =
* Use 5 Headlines, generate animated GIF
* Make use of GifMerge.class.php

= 0.2 =
* Added date() to image and made it optional (thx to pcDummy)
* Administrative interface
* Code cleanup

= 0.1 =
* Added basic Support for Polyglot (hack)
* Initial release
