+++
title = "Static to responsive in five hours"
description = "Responsive web design has been giving me sleepless nights, but I finally overcame the fear with a little help from Zurb’s Foundation framework"
date = 2013-01-24
[taxonomies]
tags = ["web design"]
+++

The thought of making my blog responsive has always struck fear where it wasn’t wanted. Fear, that is, of breaking my blog, discovering I didn’t have the necessary back-ups to reassemble the static status quo, and having to start over.

When I went to bed last night, the resulting brain activity didn’t bode well. Combined with the knowledge that an imminent increase in workload would delay any meaningful attempt to make my blog responsive, sleep proved impossible.

I got up at 2am. By around 7am I was finished, although only in the sense that the blog can live and breath on its own. I can deal with any final tweaks – in particular to the header, navigation and footer – as mini projects.

Numerous tools helped me along the way, including Coda 2, but it was [Zurb’s Foundation](http://foundation.zurb.com) framework that performed most of the magic. The site was fully responsive within an hour. The remaining four hours, I spent tweaking Foundation’s settings and editing in [Sass](http://sass-lang.com).

### Adaptive–responsive, not just responsive

The result is a hybrid adaptive–responsive approach. As a control freak, and one with an interest in typography, I was never going to relinquish control over the type measure used in the main blog. Instead, I opted to apply a `max-width` of 556px to the blog’s main container to prevent it resizing (growing bigger) once the first breakpoint at 767px was reached. As a result, text only starts to reflow when the device width is safely below the small tablet portrait width of around 600px. In other words, the measure of the main blog only changes on mobile screens.

Some quick tests in Safari, Chrome, Firefox, Opera and IE (9) on the desktop, and on the iPhone and iPad, suggest the site is working as expected.

There is still a lot to do, but what remains is cosmetic rather than structural. Maybe now I can concentrate on the most important aspect of having a blog – blogging.

In future, I’ll post in more detail about some of the decisions I took. In the meantime, you might like to – no, I know you’d love to – subscribe to my RSS feed, below. If you have something to add, please feel free to comment or say it on Twitter. Time to walk the dog.
