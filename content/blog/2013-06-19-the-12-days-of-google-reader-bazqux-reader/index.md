+++
title = "The 12 days of Google Reader: BazQux Reader"
description = "The 12 days of Google Reader is a series of posts that explores options for RSS users in a post-Google Reader world. First up, BazQux Reader"
date = 2013-06-19
[taxonomies]
tags = ["apps", "Bazquz Reader", "RSS"]
+++

First up, [BazQux](https://bazqux.com). You’ve probably never heard of it, and nor had I up until a couple of days ago. As for the name, don’t ask, even the developer says it has no meaning. But what’s intriguing about BazQux is that its interface is so like the Google Reader of old; you feel at home immediately. It’s also fast, blazingly so.

### Who’s behind BazQux?

BazQux is the work of Moscow-based Haskell programmer Vladimir Shabanov, known to his friends as *Владимир Шабанов*. Information about Shabanov is thin on the ground, but according to his G+ profile he likes to ‘develop useful tools’. He’s come to the right place. And BazQux is certainly one of those.

BazQux offers a free 30-day trial, so there are very few hoops to jump through before you’re up and running. Sign in with Facebook, Twitter, Google+ or OpenID – there’s no email/password option – and you’re prompted to import your feeds.

{{ image(path="gr-bazqux-import-600-io.jpg", caption="BazQux Reader: Import from Google Reader or upload an OPML file") }}

I clicked *Import your subscriptions from Google Reader* and BazQux’s browser filled in an instant, with each feed assigned to folders that matched those I’d set up in GR. There’s also the option to import your ‘subscriptions.xml’ file, the one that’s downloaded when you use Google Takeout.

{{ image(path="gr-bazqux-list-compact-600-io.jpg", caption="BazQux Reader: List view (compact), very like GR’s list view. There’s also normal, which shows the title, author, a line of body copy and comment numbers, if any, and ultra-compact, which is too tight for my liking") }}

In all there are five views to choose from: expanded, expanded without comments, magazine, mosaic and list. Further, there are three interpretations of the list view: normal (with a couple of lines of text below the title), compact (like the old GR list view) and ultra-compact (crazy tight and unreadable, but I guess some like it or it wouldn’t be there).

### Interface

I don’t generally consume my feeds in the browser. I read them on my iPad (Mr Reader), occasionally on my iPhone (Reeder), and very rarely on my Mac (Reeder). The web interface is like my car’s engine – it just ticks away in the background doing what it’s supposed to do (most of the time, anyway).

BazQux’s web interface is clean and functional. It also includes a set of keyboard shortcuts similar to those in GR. I like using keyboard shortcuts – when I can remember them. For a quick reminder of the options available to you in BazQux, just tap `h`.

{{ image(path="gr-bazqux-topbar-600-io.jpg", caption="BazQux Reader: mousers should be happy with the range of options available in the top bar") }}

In the top bar you can (left to right): add a subscription, sort, search, change the view, mark all as read, skip, ignore, toggle article view[^1], jump forward and backward through feed items, and access settings. In my case, above, there’s also a handy reminder that the free trial ends soon.

### Sharing

The social sharing options per feed are Twitter, Facebook, Google+ and Tumblr. There’s also an option to send links to articles by email. The bookmarking options are Pinboard, Delicious, Evernote, Pocket, Readability and Instapaper. Enough to cover most needs I would have thought; they definitely cover mine.

### Search

Search, accessible using `/` as a shortcut key, delves deep, returning all feed items that contain your query, whether in the title, in the article body, or among its tags. Note that tags are those added by the original author; you can’t add your own tags within BazQux, except, for example, when bookmarking a feed item using one of the built-in sharing services.

BazQux also has some useful filters to aid you in your search:

* **img:true** to show only messages with images
* **author:john** to filter specific author
* **subject:bazqux** for messages with subjects containing "bazqux"
* **tag:reader** if you need to filter by tag
* **comment:true** or **comment:false** to show comments or posts only
* **(bazqux *or* rss) *and not* google** for more complex queries.

### Cost

Having experienced the trial, the developer kindly lets you decide what the service is worth to you. The options are $9, $19 and $29; Feed Wrangler, another of the readers we will look at, also charges $19. Unfortunately, Feed Wrangler takes a pay-now-try-later approach. Payments to BazQux are processed securely by FastSpring.

### Issues

The biggest issue for any standalone feed-reading service will be app support. Shabanov’s smart approach – putting out an API that closely matches GR’s, the API that developers are already familiar with – is paying off. BazQux will be supported in the next releases of two of the most popular iOS RSS clients, Mr. Reader for iPad (since closed) and Feeddler for iPhone. It is also supported on the Android platform, by gReader. At the time of writing, Reeder, SlowFeeds and Newsify had given no indication that they would support BazQux, but that’s not to say they won’t. 

Finally, it’s important to note that getting your feeds out of BazQux (Settings > Subscriptions > Export OPML) is just as easy as it is to import them. Why not take advantage of the 30-day trial? If it’s not to your liking, or your favourite app doesn’t add support during that time, you can always take your feeds elsewhere.

**Tomorrow:** iPad app Mr Reader.