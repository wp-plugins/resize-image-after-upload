=== Resize Image After Upload ===
Contributors: jepsonrae, huiz
Donate link: http://www.jepsonrae.com/
Tags: image, plugin, resize, upload
Requires at least: 2.6
Tested up to: 3.4.2
Stable tag: 1.0.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This plugin resizes uploaded images to a given width after uploading, discarding the original uploaded file in the process.

== Description ==

The plugin affects the uploaded image after it is uploaded. Straight after it is uploaded, it it resized physically to the given width. There is no original image left, nor a backup made. This is deliberate to prevent wasted server space from enormous image files being stored. Unfortunately, this causes EXIF information to be lost.

A lot of WordPress users or developers who use WordPress as a CMS and want to configure it for easy use, would like to have an option to resize uploaded images. Some images come straight from digital cameras and exceed 4000 pixels in width. So it would be nice to reduce that to the max width you use inside your WordPress theme.

If you would like to keep control of perfect sharpness when resizing, it would be better use photo editing tools on your computer, not a script like this.

The plugin uses a class originally from Jacob Wyke (www.redvodkajelly.com) and is a direct update of another plugin called Resize at Upload which is no longer maintained.

== Installation ==

1. Upload the plugin 'resize-image-after-upload' to the '/wp-content/plugins/' directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Make your settings through the 'Settings > Resize Image Upload' menu in WordPress
4. Upload images while writing posts and pages.

== Screenshots ==

1. Full preview of the settings screen

== Frequently Asked Questions == 

Q. Why not reduce images in height?
A. The reason I wrote the plugin was to stop breaking the layout with
   images that are to large. Height is not always an issue. Maybe in
   future this option will be added.

Q. Does it keep my EXIF data?
A. No. Although it is programmatically possible to extract that data 
   first and put it somewhere in the metadata, which is not implemented
   off course, but a possibility, the data is lost in the process of
   resizing.

== Changelog ==

= 1.0 =
* Created initial plugin.