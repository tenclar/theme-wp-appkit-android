<!--
Theme Name: theme-wp-appkit-android
Description: A clean and simple iOS app news theme featuring: back button, content refresh, custom post types, embeds, infinite list, network detection, off-canvas menu, offline content, pages, posts, responsive, touch, transitions
Version: 1.0.7
Theme URI: https://github.com/tenclar/theme-wp-appkit-android
Author: Uncategorized Creations, tenclar Modify		
Author URI: http://uncategorized-creations.com	
WP-AppKit Version Required: >= 0.6
License: GPL-2.0+
License URI: http://www.gnu.org/licenses/gpl-2.0.txt
Copyright: 2016 Uncategorized Creations	
-->


# theme-wp-appkit-android
Tema para plugin wp-appkit android
theme-wp-appkit-android is a theme for mobile apps and Progressive Web Apps (PWA) built with WP-AppKit, a WordPress plugin to create mobile apps connected to WordPress (more on that at http://getwpappkit.com).

# Installation

Please note that beginning with WP-AppKit 0.6, Q for Android is pre-installed on plugin activation as the default theme for Android applications.

Download WP-AppKit: https://github.com/uncatcrea/wp-appkit/releases
Install WP-AppKit as you would do for any other WordPress plugins (ie. drop the plugin folder in /wp-content/plugins)
Activate WP-AppKit using the Plugins WordPress admin panel. (Browse the Installed Plugins list and click the Activate link of WP-AppKit.)
Now you should have a brand new /wp-content/themes-wp-appkit folder (yes, this is where app themes are stored)
Download the theme-wp-appkit-android from this repository and drop its folder in /wp-content/themes-wp-appkit
In WordPress, use the WP-AppKit admin panel to create a new app and choose one of the themes in the Appearance box
From there you're free to test in your browser (using the Chrome's Emulation Mode) or directly try to compile
If new to WP-AppKit, you might want to read this article: http://uncategorized-creations.com/1212/compiling-app-using-wp-appkit-phonegap-build/.

# Theme's Overview
## What's implemented

At the moment, theme-wp-appkit-android theme implements:

<ul>
<li>A shiny material design UI (including transitions and ripple effect)</li>
<li>Off-canvas menu (you can update it in the app's edit panel)</li>
<li>Archive template (eg. post list) with infinite post list</li>
<li>Single template (eg. a post) with the most common HTML elements (eg. strong, em, blockquote...)</li>
<li>Responsive embeds</li>
<li>The refresh process</li>
<li>Offline cache (meaning that you can read loaded posts offline)</li>
<li>Post thumbnail captions and subhead support</li>
<li>A responsive interface</li>
</ul>

# Android UI

<ul>
<li>Ripple effect</li>
<li>Status bar color matches the theme</li>
<li>Android spinner</li>

</ul>


# Cordova Plugins

theme-wp-appkit-android relies on Cordova plugins to:
<ul>
<li>Customize the iOS status bar: https://github.com/apache/cordova-plugin-statusbar</li>
<li>Open external links in default browser (ie. Chrome): https://github.com/apache/cordova-plugin-inappbrowser</li>
</ul>
WP-AppKit export function adds these plugins automatically to your config.xml file. If you don't use the export, make sure to add them in order the theme to be able to work properly.

# Responsive Images
theme-wp-appkit-android hooks into the WP-AppKit web services to modify the source code of images in the post content. It eases the way to style the responsive images later. See prepare-content.php in the php folder of the themes.

# Thumbnail Captions and Subheads
theme-wp-appkit-android into the WP-AppKit web services to modify add thumbnail captions and subheads (if available) in the post content. See add-custom-data.php in the php folder of the themes. Note that subheads are expected as a post custom field.
