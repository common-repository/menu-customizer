=== Menu Customizer ===
Contributors: celloexpressions, wordpressdotorg
Tags: menus, custom menus, customizer, theme customizer, gsoc
Requires at least: 4.3-alpha-32764
Tested up to: 4.3-alpha-32806
Stable tag: 0.6
License: GPLv2

Manage your Menus in the Customizer. WordPress core feature-plugin merged in WordPress 4.3.

== Description ==
**This plugin has been merged into WordPress core as of version 4.3.**

This plugin is a WordPress core feature-plugin and a former Google Summer of Code 2014 project. See the <a href="http://make.wordpress.org/core/tag/menu-customizer/">updates on Make WordPress Core</a> for more information.

The Menu Customizer adds custom menu management to the Customizer. The plugin requires WordPress 4.3-alpha-32764 or higher and has been tentatively approved for merge into core for version 4.3.

Menu Customizer fixes some significant problems with the existing approach to menu management in core, particularly around scaling. Note that its scope carefully excludes fundamental changes with the menus paradigms; rather, the goal of this project is to modernize the menu management experience so that the UX can be iterated on more reasonably. Most importantly, Menu Customizer allows you to live-preview changes to your menus before they're published.

If you're interested in contributing to this project, stay tuned to http://make.wordpress.org/core for updates, or ping @celloexpressions on <a href="http://chat.wordpress.org/">WordPress core Slack</a>. Development is happening on GitHub: https://github.com/voldemortensen/menu-customizer.

= Core Patches =
Several improvements to the Customizer are also in the works as a part of this project, in the form of core patches (for example, the Panels API, and the still in-progress APIs for dynamically-added controls and sections). See <a href="http://make.wordpress.org/core/tag/customize">Customizer posts on make/core</a> for details.

== Installation ==
1. Take the easy route and install through the WordPress plugin installer OR
1. Download the .zip file and upload the unzipped folder to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. Visit the Customizer (Appearance -> Customize) to customize your menus with live previews.

== Changelog ==
See full details here: https://plugins.trac.wordpress.org/log/menu-customizer
= 0.6 =
* Refactor internals to leverage Customizer settings for menu items and menus
* Introduce drag & drop submenus
* Add unit tests
* Countless fixes for various details
* Update 4.3 alpha/trunk to latest before updating the plugin

= 0.5 =
* Many, many fixes and improvements, see the full changelog and a summary on github: https://github.com/voldemortensen/menu-customizer/issues?q=is%3Aissue+is%3Aclosed+milestone%3A0.5
* Note that WordPress 4.3 alpha is now required.

= 0.4 =
* In-Customizer previewing of “original” menu item links.
* A redesign of the screen options popup.
* Add theme location checkboxes within menu sections (which fully cross-sync with the menu locations section).
* Theme locations listed within menu section names.
* Menus can only be deleted when they aren’t assigned to any locations.
* Available menu item searching, and a first-pass redesign of the available menu items panel to match the new look for core in #31336 (more to come here).
* Integration of the existing core theme location controls into the plugin.
* Props to @celloexpressinos, @valendesigns, @voldemortensen, and @folletto.

= 0.3 =
* PHP 5.2 support.
* Refactor PHP codebase to be object-oriented.
* General code & inline documentation cleanup.
* Lazy-load menu item controls when their containing menu is opened.
* Lazy-load all items in the available menu item panel.
* Redesign menu deletion.
* Redesign menu item list views with less spacing for a clearer visual experience.
* Redesign the add-new-menu section to be displayed like a button.
* Handle errors in ajax actions with user notices.
* UI updates for http://core.trac.wordpress.org/ticket/31336, which will become required soon.
* Props @celloexpressions, @valendesigns, @voldemortensen, @westonruter, and @kucrut

= 0.2 =
* Leverage all of the new core Customizer API features that were developed in WordPress 4.1. 4.1 is required, and while we'll try to keep the plugin compatible with 4.1 for as long as possible, we may bump the requirement to 4.2-alpha eventually. Menu Customizer development was on hold while the 4.1 Customizer work happened; we'll pick things back up here now that the needed core APIs are mostly in place. If all goes well, depending on contributor interest and release timing, we may be able to propose Menu Customizer for core merge in WordPress 4.2.
* Adding new menus should work without a page refresh now.
* Menu item controls are rendered from JS templates now, both on init and when they're added dynamically. This should further improve performance and scalability, and is also generally awesome.
* While not particularly relevant given the other changes, compatibility fixes for WordPress 4.1 (including a fatal error) were also made.
* Props to @westonruter for making a couple of quick passes through the code and contributing patches to clean up the new JS implementation.

= 0.1 =
* Extensive code cleanup.
* First pass at sub-menus, via the buttons in the "reorder" mode.
* Panel tweaks to sync with changes in WordPress core.
* End of GSoC coding period.

= 0.0.6 =
* Implement live-previewing of menus and menu items.
* Use core templating functions in JS.
* Visual improvements to the add-menu-items panel, with scrolling contained within available-item-type sections. More to come here on the code side.

= 0.0.5 =
* Add/delete Menus
* Menu item & menu data is now saved in a scalable way.

= 0.0.4 =
* Add-menu-items
* Use panels

= 0.0.3 =
* Initial commit.

== Upgrade Notice ==
= 0.2 =
* Leverage new WordPress core APIs in WordPress 4.1, fix 4.1 compatibility.
