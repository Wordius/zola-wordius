+++
title = "Custom dictionary search for Alfred"
description = "A custom search scheme for Alfred that returns results from Merriam-Webster’s online dictionary"
date = 2013-03-24
[taxonomies]
tags = ["apps", "Alfred"]
+++

When I upgraded to [Alfred 2](http://www.alfredapp.com), there were a number of things that didn’t transfer well from Alfred 1. My dictionary search was one of them.

This morning I had a trawl around the web to find which online dictionary gave the best results. Top, by a long shot, was [Merriam-Webster](http://www.merriam-webster.com) (available from [Amazon UK](http://amzn.to/ZLdVJs) or [Indiebound US](http://www.indiebound.org/book/9781476705040?aff=Wordius)), which also includes tabbed access to a thesaurus and encyclopedia.

My custom search uses the keyword ‘dict’. In the search URL, below, ‘{query}’ will be replaced by your search term.

`http://www.merriam-webster.com/dictionary/{query}`

Alfred comes with many built-in web searches. For more about creating and using custom web searches in Alfred, see the [support pages](http://support.alfredapp.com/features:web-search).