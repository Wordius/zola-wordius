+++
title = "Jekyll and the IndieWeb"
description = "Creating an IndieWeb-compliant website with Jekyll"
date = 2015-01-06
[taxonomies]
tags = ["Jekyll", "IndieWeb"]
+++

When this site switched to [Jekyll](http://jekyllrb.com) back in August 2014, the overwhelming reason for the move was a desire to return to a static, file-based blog. But there was a nagging suspicion that I would struggle to incorporate the principles of the [IndieWeb](http://indiewebcamp.com) using Jekyll. That was never an issue with WordPress where there’s a plugin for everything. But the swathe of plugins I had already added to my site was one of the reasons I became disenchanted with WordPress for my personal blog in the first place, although I continue to use that CMS to develop other sites.  

Since the switch to Jekyll, when time allowed, I have adjusted the mark-up to make the content more IndieWeb-compliant, such as including an [h-card](http://indiewebcamp.com/h-card) and marking up posts using [h-entries](http://indiewebcamp.com/h-entry). [IndieWebify](http://indiewebify.me) proved invaluable in setting up and validating my h-card and h-entry mark-up. Recently, I added [Webmentions](http://indiewebcamp.com/Webmention) to posts, making visible any interactions with posts I share, such as ‘Likes’ and ‘Retweets’ (Reposts). This site is also [IndieAuth](https://indieauth.com)-enabled to some extent.

### Webmentions

To implement Webmentions on this site, I used Pelle Wesseman’s [Herokuapp service](https://webmention.herokuapp.com). Although there were some initial, self-inflicted issues getting it up and running, Wesseman’s Webmentions’ service couldn’t be easier to set up.

Add the following code to the `head` of your Jekyll site:

`<script src="https://gist.github.com/Wordius/62b6886d1e78cbec0500.js"></script>`

Then add the following script to your Jekyll layout files, usually default.html right after `{ content }`, where you would like to output any Webmentions:

`<script src="https://gist.github.com/Wordius/375594bd01ba6ff55e5e.js"></script>`

Lastly, you will need to do some styling. When Webmentions appear on your site, they are marked up like this:

`<script src="https://gist.github.com/Wordius/5236913b9ccc2ce82314.js"></script>`

Use the classes in the code above to add some nice styles before updating your live site.

### Posseing (Publish [on your] Own Site, Syndicate Elsewhere)

Long term, the aim is for this site to become the sole source of all of my content, whether blog posts, pictures, tweets or Facebook posts – the latter two ‘possed’ to the silos rather than posted directly. To that end, I have created custom layouts for posts, notes (tweets) and pictures. To date I have only added one picture and one note while I try to figure out the best way to posse. Posting every tweet to my blog as a note and manually posseing each one to Twitter would be a huge, time-wasting undertaking using Jekyll, and a route I don’t plan on taking. So, until I figure out a better way I will only be posseing long-form posts, simply by using the Twitter share button that appears at the bottom of each post.   

### All sound a bit too much effort?

The best, out-of-the-box IndieWeb solution I have come across is [Known](https://withknown.com). No coding experience is required if you use the hosted solution, but if you own a domain and feel comfortable uploading files to your server, you might like to download the [self-hosted version of Known](https://withknown.com/developers/). My only reservation is how long Known will stick around, so I will continue to update my Jekyll blog.

Another effort to look out for, which is not directly associated with the IndieWeb but follows many of the same principles, is [ind.ie](https://ind.ie). The team at ind.ie are building a number of tools that together make up the Indienet, a post-cloud platform where *you* are the network. According to the Ind.ie website:

> “The Indienet is a peer-to-peer social network that sits on top of the Internet and overlaps with the Web.”
>
> – [It’s time to move beyond the clouds](https://ind.ie/stratosphere)

The future for all of these technologies largely depends on how widely they are adopted. If they are simply tools aimed at developers, then they’re not going to get very far. If, on the other hand, they are built to be the kind of tools your granny could use, much as Known’s hosted platform is, wider adoption is a real possibility.

Exciting times lie ahead in 2015.