+++
title = "Create a sitemap for your Jekyll blog without using a plugin"
description = "A simple solution for adding a sitemap to your Jekyll blog"
date = 2015-01-08
[taxonomies]
tags = ["Jekyll", "sitemaps"]
+++

The development of this Jekyll blog continues with the addition of a sitemap, for which thanks to [havvg](https://github.com/havvg/havvg.github.com/blob/master/sitemap.xml).

Simply create a file called `sitemap.xml` in the root of your Jekyll site and add the following code:

`<script src="https://gist.github.com/USERNAME/506f037ad499cb93de2a.js"></script>`

My first attempt to create a sitemap for this site using [Michael Levin’s plugin](https://github.com/kinnetica/jekyll-plugins), as recommended on Jekyll’s [plugin page](http://jekyllrb.com/docs/plugins/), failed. I have no idea if it was something else I did, but after adding the plugin to my site and running `jekyll serve`, the site failed to regenerate. So I deleted Levin’s plugin and used the method above instead.

