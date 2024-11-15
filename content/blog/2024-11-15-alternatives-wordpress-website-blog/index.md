
+++
title = "Alternatives to WordPress for your website or blog"
description = "If you’re looking to exit WordPress, given Mullenweg’s recent Musk-like transformation, here are some alternative solutions for your blog or website"
date = 2024-11-15
[taxonomies]
tags = ["markdown", "zola", "static site generators"]
+++


<figure>
        <img src="wp-spitting-dummy-bw.png" srcset="wp-spitting-dummy-bw.png 1024w, wp-spitting-dummy-bw.avif 1024w, wp-spitting-dummy-bw.heic 1024w, wp-spitting-dummy-bw.webp 1024w" alt="caption" />
</figure>

With all the controversy surrounding WordPress at the moment, it wouldn’t surprise me if there were people out there looking to jump ship. I think Mat Mullenweg spat his dummy out, personally; he’s like a smaller version of Elon Musk, and everyone knows what a deluded individual (I’m being nice here) he is.

These are the options I have up to now. I haven’t tested them all. The furthest I have gone with most is to download, install from Terminal and look at the basics of how they work. Nothing beyond that, apart from Eleventy, Kirby and Jekyll. Eleventy looked like a workable solution till I got down to the nitty-gritty. The nitty-gritty did not look good, certainly for someone who might be considered a serial cut-and-paster.

Kirby, back in around 2013 when it was on version 1 or 2 – I can’t remember which – was also used for this blog but an upgrade broke my system (or train of thought) and I never went back. Similarly with Jekyll, there was an issue with Ruby I couldn’t fix so that was put to one side and this site went back to WordPress. So what are the alternatives to WordPress? 

### ClassicPress

Not a million miles away from WordPress is ClassicPress, which is like WP used to be with its classic environment before it became wedded to its block editor concept (and AI). Even when this website was built using WP I did not like the block editor, always reverting to the classic environment via a plugin. If I’d known about ClassicPress, I would have switched.

**More about** [ClassicPress](https://www.classicpress.net/get-classicpress/)

This is not a huge list of static site generators by any means. These are the ones I’ve had a quick go with. Most SSGs are free to use. Only a few, such as Kirby, make a charge.

### Zola

Zola is my current favourite, and what this site is built with. It is simple to use and looks quite straightforward from the outset. I use it, so it has to be simple. Even the file system you are left with after install (see image below) looks simple. It’s worth noting here that I did not use any themes, plugins or macros to create this site; all I have is the content, a bunch of templates and a CSS file; the templates and CSS files do most of the work.

<figure>
        <img src="screenshot-zola-1024.png" srcset="screenshot-zola-1024.png 1024w, screenshot-zola-1024.avif 1024w, screenshot-zola-1024.heic 1024w, screenshot-zola-1024.webp 1024w" alt="Zola’s simple site structure" />
        <figcaption>Zola’s simple site structure is contained in two files and six folders</figcaption>
</figure>

Two files and six folders represent the full workings of Zola. First there’s config.toml, which is your configuration file then netlfiy.toml, which you only generate if you intend to use Netlify. The folders contain:

- **content** – all sections (blog, etc.) and pages in markdown format.
- **public** – the generated site.
- **sass** – if using sass files; I don’t, and I have not tried to delete the folder.
- **static** – your static files, such as CSS, site logos, images, etc.
- **templates** – all your templates in html format. 
- **themes** – if using a theme; again, I have left it alone in case it’s presence is necessary for Zola to work.

Zola is as simple as that, where most other static site generators come with a whole host of files in whatever language you care to name, such as PHP or JS. I guess that’s a result of Zola being made from a single binary.

Note that this site is served up on Netlify with Github acting as storage. I have a number of Europe-based alternatives to explore before I bring it closer to home.  

**More about** [Zola](https://getzola.org)

### Astro 

Astro is a JavaScript web framework optimised for building fast, content-driven websites. Whether you’re building a marketing site, a blog or an e-commerce site, Astro can do it, so the marketing blurb says. There is also a useful [tutorial](https://docs.astro.build/en/tutorial/0-introduction/) which, in the case of a blog, should give you a chance to explore how it all works. You can complete it all in one go or in stages. It saves where you’ve got to after each stage.

**More about** [Astro](https://astro.build)

### Bludit

Bludit describes itself as a simple, fast, secure, flat-file CMS. It uses files in JSON format to store the content, so there’s no need to install or configure a database. It supports markdown, themes, plug-ins and is SEO friendly. Note that you have to deactivate the TinyMCE editor, available by default, and activate the SimpleMDE plugin to enable markdown. 

And, yes, it has it’s own built-in admin system so there’s no need to open Terminal or any other CLI for that matter.

I’d already installed Zola by the time I came across this, and already exhausted my time in building, so I haven’t looked further into using Bludit. On the face of jt, though, Bludit looks like a no-brainer; it even connects and posts direct to Mastodon or Friendica.

**More about** [Bludit](https://docs.bludit.com/en/getting-started/installation-guide)

### Eleventy

Template languages include HTML and markdown, along with Javascript, HAML, WebC, Nunjucks, Liquid, Handlebars, Mustache, EJS, Pug… It’s easy to see why I fell out with Eleventy; I know some HTML and CSS, but I speak most other computer languages like a rusty, Spanish-speaking Englishman. It’s an SSG that is aimed at developers and, unless you speak their language(s), and fluently, I might add, you might as well forget it. There is a useful Discord community if you happen to speak their language, but it is definitely not a tool I’d recommend for a cut-and-paster like me.

**More about** [Eleventy](https://www.11ty.dev)

### Grav

Described as a modern, open-source flat-file CMS. If you haven’t heard of Grav, it was voted the best flat-file CMS in 2021, as well as a number of previous years.  Like Bludit, Grav comes with its own admin panel. The Grav admin plugin provides a simple interface to make configuration and content creation easy.

Definitely worth a look.

**More about** [Grav](https://getgrav.org/downloads)

### Hugo

Hugo is described as ‘one of the most popular open-source static site generators. With its amazing speed and flexibility, Hugo makes building websites fun again’. All of which may be true, but all I was interested in does it do Markdown. And the answer is: yes. Markdown even gets its own superpowers in the form of Hugo’s shortcodes.

**More about** [Hugo](https://gohugo.io)

### Middleman

Despite having my ups and downs with the Ruby language – mostly downs – I thought Middleman might be interesting. It uses a templating language called ERB, which if you’ve never heard of it is like HTML with variables. That’s where my interest in it waned, I’m afraid. I link it here only to show it as an alternative.

**More about** [Middleman](https://middlemanapp.com/basics/install/)

### Pelican

Pelican is a static site generator that requires no database or server-side logic. Languages include Python and Jinja2, and it even allows the importing of sites from WordPress or RSS. I like penguins is all I can say.

**More about** [Pelican](https://getpelican.com)

### Quartz

Quartz is a set of tools that helps you publish your digital garden and notes as a website for free. It is a fast static-site generator that transforms markdown content into fully functional websites.

The developers recommend that you use [Obsidian](https://obsidian.md/) as a way to edit and maintain Quartz. Obsidian comes with a nice editor and graphical interface to preview, edit, and link your local files and attachments.

**More about** [Quartz](https://github.com/jackyzha0/quartz)

There are many others. I’m quite satisfied with Zola, but, given my propensity for switching, Bludit or Grav look like the natural choices.

[Jamstack](https://jamstack.org/generators/) has a fuller list if you want to spend a sizeable chunk of what remains of your life looking at static site generators.  