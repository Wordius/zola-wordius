+++
title = "WordPress plugins: My ‘Core 10’"
description = "Some WordPress plugins crop up time and again in every site I build. These are my ‘Core 10’"
date = 2013-07-05
[taxonomies]
tags = ["web design", "WordPress"]
+++

When developing sites in WordPress, it’s useful to have a set of core plugins,[^1] the ones you turn to time and again on most every site that comes your way. The list below contains my *Core 10*. These are the plugins that help me during development and many also benefit site users long after deployment.

### AccessQontrol

AccessQontrol comes in handy when you’re testing sites prior to going live and when performing maintenance. AccessQontrol is a simple plugin that allows you to serve ‘This site is down for maintenance’ or ‘Launching soon’ type messages to site visitors while allowing specified users, such as Admin (for security reasons, you shouldn’t actually have a user called ‘Admin’), to view the site and check the results of their handiwork.

Download from the developer’s site and store the AccessQontrol files in a ‘WordPress > Plugins’ folder on your computer. That way you can upload it when needed and apply any updates using the WP plugins’ panel. 

<p class="small">
<strong>Rating</strong> Not available – <strong>Download</strong> <a href="http://meandmymac.net/430/accessqontrol-12/">AccessQontrol</a></p>

### Admin Management Xtended

Admin Management Xtended allows you to manage posts and pages without having to open them in a new tab or window. The official plugin page says:

> [Admin Management Xtended] adds some icons to the posts/pages management panel with AJAX-driven CMS-known functions like toggling post/page visibility, changing publication date and title without having to open the edit screens or reload the page, plus changing page order with drag’n’drop, inline category management and inline tag management, plus much more.

This [Vimeo video](https://vimeo.com/9598749#at=0) provides a demo of some of AMX’s key features.

<p class="small">
<strong>Rating</strong> 4.2/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/admin-management-xtended/">Admin Management Xtended</a>
</p>

### Dynamic Widgets

The developer says: 

> Dynamic Widgets gives you full control on which pages your widgets will appear. It lets you dynamicly show or hide widgets on WordPress pages…

… whether category pages, tag pages, post-type pages, and on and on. Dynamic Widgets is one of those plugins that saves a lot of time, an awful lot of time.

<p class="small">
<strong>Rating</strong> 4.8/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/dynamic-widgets/">Dynamic Widgets</a>
</p>

### Login Lockdown

Hackers are known to exploit, or attempt to exploit, WordPress installations using [brute-force attacks](http://www.forbes.com/sites/anthonykosner/2013/04/13/wordpress-under-attack-how-to-avoid-the-coming-botnet/). Login Lockdown limits the number of login attempts from a specific IP range during a user-specified timeframe, stopping brute-force attacks in their tracks. 

The developer says:

> Login LockDown records the IP address and timestamp of every failed login attempt. If more than a certain number of attempts are detected within a short period of time from the same IP range, then the login function is disabled for all requests from that range.

There’s a warning in the Plugin Directory that Login Lockdown has not been updated in over two years. I included Login Lockdown in my *Core 10* a couple of months ago, which makes it the most recent addition. It works and I haven’t experienced any conflicts, many WordPress moons since it was last updated; I’m running the latest version of WordPress, 3.5.2.

<p class="small">
<strong>Rating</strong> 4.6/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/login-lockdown/">Login Lockdown</a>
</p>

### Jetpack by WordPress.com

I don’t make full use of this giant of a plugin – not yet anyway – but I really like the *stats* feature it adds to the WP dashboard.

When I last counted, there were 26 other features in Jetpack, including notifications, sharing, carousels, shortcodes and a URL shortener. Dive in.

<p class="small">
<strong>Rating</strong> 3.8/5.0 stars – <strong>Download</strong> <a href="http://jetpack.me">Jetpack</a>
</p>

### Reveal IDs

Probably the first, and the simplest, plugin to make it into my *Core 10*. When WordPress 2.5 was released, it removed IDs from all admin pages. Reveal IDs reinstates them. That’s it.

<p class="small">
<strong>Rating</strong> 4.6/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/reveal-ids-for-wp-admin-25/">Reveal IDs</a>
</p>

### W3 Total Cache

I tried a number of caching plugins before settling on W3 Total Cache. Caching pages and resources improves page speed and, in doing so, delivers a better user experience.

W3 Total Cache has a vast number of features. While I don’t claim to understand most of them, the few that I have enabled – page caching, minifying, browser caching and object caching – make my pages render more quickly. 

WP Beginner has a useful article for newcomers that describes [how to install and set up W3 Total Cache](http://www.wpbeginner.com/plugins/how-to-install-and-setup-w3-total-cache-for-beginners/).

<p class="small">
<strong>Rating</strong> 4.6/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/w3-total-cache/">W3 Total Cache</a>
</p>

### Widgets Reloaded

Put simply, Widgets Reloaded replaces many of WordPress’s default widgets with versions that offer greater control.

The widgets it replaces are: Archives, Authors, Bookmarks (Links), Calendar, Categories, Navigation Menu, Pages, Search and Tags.

Widgets Reloaded is another plugin that hasn’t been updated in over two years. Despite the warning on the Plugin Directory, Widgets Reloaded works perfectly well in the latest version of WordPress, 3.5.2.

<p class="small">
<strong>Rating</strong> 4.4/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/widgets-reloaded/">Widgets Reloaded</a>
</p>

### WordPress SEO

Joost de Valk, of Yoast, wrote his SEO plugin to improve every area of a WordPress site’s SEO. 

Web designer Paul Boag has been sceptical about the value of SEO. Earlier this year he conducted a four-month experiment, using Yoast’s WordPress SEO plugin, to find out for sure. He wrote about his experiment in [Perhaps SEO isn’t all bad](http://boagworld.com/marketing/perhaps-seo-isnt-all-bad/).

For a detailed explanation of how to set up and use the WordPress SEO plugin, read Yoast’s [Definitive guide to higher rankings for WordPress sites](http://yoast.com/articles/wordpress-seo/).

<p class="small">
<strong>Rating</strong> 4.7/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/wordpress-seo/">WordPress SEO</a>
</p>

### BackWPup

After you’ve put in all the hard work and your site is up and running, the last thing you want to do is lose it.

BackWPup allows you to “schedule easy, and complete automatic backups for your WordPress installation”, providing a single .zip file that you can use to restore and install your site. Your backup file can be sent to numerous services, including my favourite, [Dropbox](http://db.tt/jw9tyCz).

Importantly, in BackWP it’s easy schedule ‘jobs’ to run at any time of day or night, and as often as you like. 

<p class="small-sans">
<strong>Rating</strong> 4.4/5.0 stars – <strong>Download</strong> <a href="http://wordpress.org/plugins/backwpup/">BackWPup</a>
</p>

### There’s more…

Of course, every site is different, but I can’t think of one where I haven’t used all of these plugins in one way or another. Everyone has their favourite plugins that simplify particular tasks; feel free to mention them in comments. If you want to recommend alternatives to any of those in my *Core 10*, I’m not precious! 

The demands of particular sites often mean that I add custom sets of plugins per site to the core set outlined above. I’ll cover the plugins that often make it into those custom sets in a future post.

[Subscribe to this site’s RSS feed](https://macminded.co.uk/atom.xml) so you don’t miss it.
