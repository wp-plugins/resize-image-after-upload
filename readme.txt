=== Resize Image After Upload ===
Contributors: iamphilrae
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=3W4M254AA3KZG
Tags: image, processing, plugin, resize, upload, resizing, optimization, optimize, optimise, optimisation, downsize
Requires at least: 3.5
Tested up to: 4.1
Stable tag: 1.7

Simple plugin to automatically resize uploaded images to within specified maximum width and height. Also has option to force recompression of JPEGs.

== Description ==

This plugin automatically resizes uploaded images (JPEG, GIF, and PNG) to within a given maximum width and/or height to reduce server space usage. This may be necessary due to the fact that images from digital cameras and smartphones can now be over 10MB each due to higher megapixel counts.

In addition, the plugin can force re-compression of uploaded JPEG images, regardless of whether they are resized or not.

Note: the resizing/recompression process will discard the original uploaded file including EXIF data.

This plugin is not intended to replace the WordPress add_image_size() function, but rather complement it. Use this plugin to ensure that no excessively large images are stored on your server, then use add_image_size() to create versions of the images suitable for positioning in your website theme.

This plugin uses standard PHP image resizing functions and will require a high amount of memory (RAM) to be allocated to PHP in your php.ini file (e.g 512MB).

== Installation ==

1. Upload the plugin 'resize-image-after-upload' to the '/wp-content/plugins/' directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Edit the max-width/max-height settings under 'Settings > Resize Image Upload'.
4. Once active, just upload images as normal and it will just work!

== Screenshots ==

1. Full preview of the settings screen.

== Changelog ==

= 1.7 =
This is a major under-the-hood release to change core workings of the plugin. The plugin still functions as normal, but the way in which it resizes images has now changed to use standard WordPress libraries. This means that should your server have better image processing libraries than the GD default (e.g. ImageMagick), then the resizing method should make use of them. This should improve the output of your resized images!

* [Update] Plugin completely re-engineered to use WP_Image_Editor when resizing images.

= 1.6.2 =
Minor maintenance release:

* [Fix] Correcting an error in the documentation.

= 1.6.1 =
Fix a few edge case bugs, I go and break the main functionality - that's life! This is a maintenance release to fix a bug.

* [Fix] Correct the logic behind which direction to perform resizing in.

= 1.6 =
This is a major maintenance release to squash a few long outstanding bugs.

* [Update] Tidied up the plugin settings page.
* [Fix] Significant number of bug fixes through extensive testing.
* [Fix] Resizing wasn't running on square images.
* [FIX] Media upload was failing for BMP images.
* [Fix] Replaced use of deprecated PHP functions with correct ones.

= 1.5 =
* [Added] Ability to force re-compression even if resize is not required.
* [Fix] Compression quality value was not adhered to.

= 1.4.2 =
* [Update] Added ability to enter a resize value of zero (0) to prevent resizing in a particular dimension.

= 1.4.1 =
* [Fix] Reverting code back to how it was in v1.3.0 after previous premature deployment of v1.4.0. Please use this version.

= 1.4 =
* [Error] Code was deployed prematurely and should not have made its way to the live repository. Please do NOT use this version.

= 1.3 =
* [Update] Added ability to set the JPEG compression quality level when JPEGs are resized. Default is 90.

= 1.2 =
* [Update] Now only runs images through the resizer if required, i.e. the image is actually larger than the max height/width.

= 1.1.1 =
* [Fix] Corrected functionality that sets default plugin options if the plugin version number changes.
* [Fix] Adds default option for max-height value.
* [Update] Updated the screenshot to include new maximum height field.
* [Update] Increased the default maximum height and width to 1200px each.

= 1.1 =
* [Update] Added ability to set maximum height (thanks @Wonderm00n).

= 1.0.1 =
* [Update] Update to read me, no feature updates unfortunately.

= 1.0 =
* [Added] Initial release.