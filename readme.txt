=== Search Placeholder Avada ===
Contributors: mlchaves
Donate link: https://ko-fi.com/marklchaves
Tags: header, avada, themefusion, search, placeholder, javascript
Requires at least: 5.3.2
Tested up to: 6.1.1
Stable tag: 2.0.0
Requires PHP: 7.2.18
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Customise the search box placeholder text for the *Avada* theme.

== Description ==

*Customise your search placeholder text!*

Search Placeholder Avada allows you to add your own custom placeholder text for Avada's search input box.

There's new support for all themes.

== Installation ==

1. Upload the contents of the plugin zip file to the `/wp-content/plugins/search-placeholder-avada` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' page in WordPress.

== Usage ==

Originally built for Avada by ThemeFusion, you can now use this on any theme. 

With version 2.0, there's built-in support for Avada and WordPress default themes. You can also use a PHP hook (filter) to add any CSS selector you need.

The plugin settings are under **Settings > Search Placeholder Avada**.

**Example Filter for Supporting Any Theme**

`
/** Search Placeholder Avada: filter for your own CSS selectors. Separate selectors with a comma. */

add_filter( 'search_placeholder_css_selectors', function() {
		return ".this-is-a-test-class, #this-is-a-test-id, .another-class";
	}
);
`

Tweak the filter for your needs. Then, add it to your child theme's `functions.php` file or use a code snippets plugin that supports adding PHP hooks.

== Frequently Asked Questions ==

= Will this plugin work for other themes? =

Yes!

Version 2.0.0 has built-in support for Avada and WordPress default themes. 

It also has new PHP filter hook for you to add any CSS selectors. That means Search Placeholder Avada can work for any theme :-)

== Screenshots ==

1. Create your custom search placeholder.
2. You set the placeholder once and it displays in every search box. 
3. Custom search placeholder text closeup.
4. Navigate to Settings > Search Placeholder Avada.
5. Plugin option settings page.

== Changelog ==

= 2.0.0 = 
* Added built-in support for WordPress' Twenty Twenty themes.
* Added filter for custom CSS selectors for any search input field.

= 1.1.0 = 
* Added code to delete placeholder option from the DB on plugin uninstall.
* Tested on WordPress 5.5 and Avada 7.0.2.

= 1.0.0 =
* First release. Tested on Avada 6.2.1 and 6.2.2.

== Upgrade Notice ==

= 1.1.0 =
* Will now clean up the sole DB option for this plugin on uninstall.

= 1.0.0 =
None

== Disclaimer ==

The Search Placeholder Avada plugin and its author are not affiliated with Avada or ThemeFusion in any way.