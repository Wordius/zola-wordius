+++
title = "How to search Google.com from within the EU"
description = "Following the EU’s ruling on Google and the ‘right to be forgotten’, here are a few ways to find everything you’re looking for, including using Alfred to search Google.com"
date = 2014-07-04
[taxonomies]
tags = ["apps", "Alfred"]
+++

For information about how the EU’s ‘right to be forgotten’ ruling came about, and the implications for press freedom, there’s a more than [adequate explanation](http://www.theguardian.com/technology/2014/may/13/right-to-be-forgotten-eu-court-google-search-results) on the *Guardian* website. The privacy ruling by the EU Court of Justice has seen many of the *Guardian*’s articles ‘disappeared’ from Google searches within the EU. Here, I will show you how to return *all* of the results you might be looking for.

There are three solutions here, but there are probably many others:

* Switch to a search engine that isn’t affected by the ruling, such as [DuckDuckGo](http://duckduckgo.com).
* Choose to search Google.com from your localised Google home page, in my case [Google.co.uk](http://google.co.uk).
* Use Alfred or LaunchBar to search Google.com.

### Switch your search engine to DuckDuckGo

[DuckDuckGo](https://duckduckgo.com) isn’t currently available in Safari’s default search options, but it will be when Apple releases [OS X Yosemite](https://www.apple.com/osx/preview/apps/) this autumn. Until that time, you can install the official [DuckDuckGo Safari extension](https://duck.co/help/desktop/safari).

The added bonus of using DuckDuckGo is that it protects your privacy by not tracking the results of your searches, unlike Google.

But if you really must use Google…

### Select Google.com from your localised Google home page

This one’s easy. Go to your localised Google home page – that’s [Google.co.uk](http://google.co.uk) in my case. Click the ‘Use Google.com’ link at the bottom right (image 1) and search away to your heart’s content.

{{ image(path="googlecom1-search-582.jpg", caption="Image 1") }}

### Search Google.com using Alfred or Launchbar

[Alfred](http://www.alfredapp.com) is a free productivity app for OS X. An in-app purchase of the Powerpack significantly increases your options, but this search snippet also works in the free version.

1. Open Alfred – the default keyboard shortcut is Alt-Space.
2. Open Alfred preferences – Command-Comma.
3. Select the ‘Features’ tab then ‘Web search’ in the left sidebar.
4. Click ‘Add Custom Search’ – bottom right of the Web Search window (image 2, below).
5. Add the following URL `https://www.google.com/search?q={query}` in the ‘Search URL’ field (image 3, below).
6. Give your Custom Search a title and a shortcut. I used ‘Search Google.com’ and ‘gcom’.
7. Click ‘Test’ to try out your search, then return to Alfred and click ‘Save’.

{{ image(path="googlecom2-alfred-web-search-custom-582.jpg", caption="Image 2") }}

{{ image(path="googlecom2-alfred-web-search-582.jpg", caption="Image 3: Alfred custom search window") }}

Now you can search Google.com simply by launching Alfred and typing ‘gcom’ followed by a space and your query.

Another launcher-type application, [LaunchBar](http://www.obdev.at/products/launchbar/index.html), provides similar functionality to Alfred, including allowing you to create your own custom searches.