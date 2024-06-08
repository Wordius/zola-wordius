+++
title = "A comparison of web-based Markdown editors"
description = "There are numerous web-based Markdown editors, but I have chosen to review the three I consider the best – Draft, Editorially and Penflip"
date = 2014-02-04
[taxonomies]
tags = ["apps", "markdown"]
+++

**Update:** <a href="http://stet.editorially.com/articles/goodbye/">Editorially has announced that it is to shut down</a> on 30 May. Users have until that date to download their data.

There are numerous web-based Markdown editors – far too many to mention here – so I’ve chosen what I consider three of the best – [Draft](https://draftin.com), [Editorially](https://editorially.com) and [Penflip](https://www.penflip.com) to review here.

One thing all three have in common is that they’re currently free to use. It takes time to maintain and develop what, on the face of it, look like simple user interfaces, but the complexity is in their simplicity. There are also other costs, such as storage, to consider. So I suspect the developers behind each of these web-based Markdown editors is working on their business model, most likely subscription based, in the background. That makes now as good a time as any to give them a try. 

Penflip is relatively new. I only heard about it last week thanks to a tweet by [Tyler Reinhard](https://twitter.com/abolishme). Draft, on the other hand, has been around for a couple of years, with occasional updates, and Editorially is progressing steadily towards its first birthday next week. Despite its baby face, Penflip is fully functional, although developer [Loren Burton](https://twitter.com/madebyloren) says he’s still “trying to nail the core”. New features, such as the ability to publish direct to a WordPress blog, for example, will follow.

So, let’s take a look under the hood. What can these web-based Markdown editors do for you, the writer?

### Key features of web-based editors

The table below outlines some of the key features you might expect to find in a web-based Markdown editor and whether or how they have been implemented in Draft, Editorially and Penflip.

| Editor | Share | Export | Publish | Import | Prev. | Vers. | Sync |
| ------ | ----- | ----- | ----- | ----- | ----- | ----- | ----- |
| Draft | Yes | Text, Markdown, HTML, Word, Google docs, PDF, Kindle, ePub | WordPress, Tumblr, others | Yes | Yes | Yes | Yes |
| Editorially | Yes | HTML, Markdown, text, LaTex, Rich text, Word, ePub | WordPress, Dropbox | Yes | Yes | Yes | No |
| Penflip | Yes | HTML, text, Word, PDF, Markdown, ePub | No | No | Yes | Yes | Yes |

### Import

If you’ve already started a project offline, or elsewhere online, Draft and Editorially let you import them. While Editorially can import text and Markdown files, Draft goes a step further by allowing you to import files from other services, such as [Dropbox](http://db.tt/jw9tyCz), Google Drive, Evernote and Box. The best bit is that Draft will also sync any changes you make back to those services. That’s an important consideration. Syncing is essential if, like me, you’ve ever had reason not to trust working in the browser.

Penflip is the only editor here that doesn’t have the facility to import existing documents, which means you’ll have to revert to good old copy and paste. That said, it does do sync, which I’ll explain later. 
 
### Collaboration

In the web-based Markdown editor market the buzzword is *collaboration* – the ability to share and receive feedback on your writing. You may already have a workflow in place to achieve this. I know I do. Publishers send raw text – whether books or articles – to a folder in Dropbox. I edit then return the article or book to Dropbox, using a naming convention to distinguish it from the original. In my case, filenames prepended with *pubx-* are good to go.

The web-based editors we’re considering here all permit collaboration. In Draft you email a link to your article to an editor, co-worker… When they’ve completed their edit, you get an email back asking you to accept or reject changes. Draft also has a paid service, Ask a Pro, where you can send your article to an experienced editor. Draft creates versions of a document every time you save.

The collaborative tools in Editorially and Penflip work in a similar way, although the latter also has an option to add contributors, or project members, from within the Penflip community – useful if all members of your ‘team’ are signed up to the service.

Editorially also has a nifty progress filter for the different stages in a document’s life – draft, reviewing, revising, copyediting and final – and offers users the ability to save versions of a document. 

Penflip creates a version of your master document for each collaborator. The collaborator cannot change the master version (unless you give them admin rather than contributor status), and changes they make in their version are submitted to you to accept or reject.

When your collaborative effort is finished, whether it’s a book, article or blog post, you need a means to move them to the next stage of your workflow.

### Export and publish 

All three editors offer an impressive range of export options – plain text, Rich text, Markdown, HTML, Word, Google docs, PDF, Kindle, ePub, LaTex – see the table above for what each editor supports.

Draft and Editorially further offer the ability to publish directly to a blog or send to Dropbox. While Editorially only supports WordPress.com blogs (or static blogs that use the Dropbox API), Draft has numerous other options, including self-hosted WordPress blogs, Tumblr, Blogger and Ghost. Penflip’s Burton says that a publishing option is planned, so we’ll have to wait and see what form that takes.

### Preview and syntax highlighting

All three editors offer document previews. But, as you can see from the screenshots below, Editorially and Penflip are the only ones to provide syntax highlighting – when you declare content to be in bold or italic in Markdown, for example, it also appears in bold. Syntax highlighting gives the reader – you – a better understanding of your document’s content and structure. In other words, it’s useful, so I don’t understand why Draft’s developer hasn’t implemented syntax highlighting.

{{ image(path="draft-582.png", caption="Draft provides a clean, uncluttered writing interface, but lacks syntax highlighting") }}

{{ image(path="editorially-582.png", caption="Editorially’s interface includes a live view of placed images") }}

{{ image(path="penflip-582.png", caption="Penflip features syntax highlighting and a handy toolbar in edit mode") }}

Note that I made the menus in Draft and Editorially visible on purpose. They are usually hidden in edit mode.
 
### Working offline

Editorially can send documents to Dropbox, but changes made to a document outside of Editorially do not sync back. And, if you go back to the online version of the document in Editorially make some changes and resend to Dropbox, the changes you made in your Dropbox version are lost. I don’t understand this choice. Two-way sync makes infinitely more sense to me, but I guess the Editorially team have their reasons.

Draft has a range of syncing options. As mentioned above, when you import a document from other cloud services, such as Dropbox, Google Drive, Evernote and Box, Draft syncs any changes you make back to the original. It’s fast and it’s painless, and it opens up the opportunity to work offline in your favourite desktop Markdown editor. Currently, I use MultiMarkdown Composer 2 most of the time, Ulysses III, some of the time.

Penflip doesn’t use Dropbox for syncing. Instead, it has adopted GitHub’s URL scheme to send ‘projects’ or documents to GitHub’s desktop app (Mac or Windows). For example, typing `github-mac://openRepo/my-project/https://www.penflip.com/username/projectname` in your browser’s address bar will launch the GitHub app on your Mac. You will be prompted to choose a location for your repository – I use a folder called ‘Penflip’ in Dropbox  – then you’re free to use the editor of your choosing. When you’re finished, commit and sync changes back to Penflip via the GitHub app. If you decide to work online in Penflip, when you make changes to the master project, repeat the above process to overwrite the repository on your desktop. If you’re familiar with GitHub and the command line, [there is a quicker way](https://www.penflip.com/Penflip/help/blob/master/WorkingOffline.txt).

Penflip’s approach is slightly more involved than Draft’s simple two-way Dropbox sync, but it works.

### Conclusion

One of the biggest doubts I have about using a web-based Markdown editor derives from that very compound adjective: *web-based*. I’ve lost count of the number of times I’ve been cut-off mid flow by a frozen browser. Whether it was an article I wrote on Medium – entire concluding paragraph lost – or a partially composed tweet, the fact is that I don’t trust the browser as a writing application – reading, yes; writing, no.

That means Editorially doesn’t make the grade at this point. Beautiful as its interface is, the ability to work offline and sync my changes back to the master is more important.

Which leaves Draft and Penflip. I want to like Draft, and I do like Draft. It feels by far the lightest of the web-based Markdown editors being reviewed here. By which I mean, its feature set isn’t overwhelming in the slightest. It’s easy to use, syncs with Dropbox, fast and efficient, and publishing to WordPress is a breeze. I particularly like the fact that you can publish your post as a draft, because I prefer to preview my posts and give them one last check prior to making them live. That all sounds positive, so why do I still have reservations? Well, while I like plain old plain text, I like unobtrusive syntax highlighting more. Editorially and Penflip both offer syntax highlighting; Draft doesn’t. It’s for this same reason that Brett Terpstra’s [nvALT](http://brettterpstra.com/projects/nvalt/) is only my day-to-day *notes* app, not my day-to-day *writing* app.

For me, the ability to work offline is just as important as having a beautiful, distraction-free user interface in which to write. Penflip offers both. Sure, it’s a bit more complicated to use, but not unreasonably so. Sure, it doesn’t currently offer publishing to WordPress, but developer Loren Burton assures me that will be added in a future release. 

Draft and Editorially have evolved and developed into fine tools, and that development process is ongoing. Penflip is young and fresh, and it too will evolve over time. But even at this early stage in its development, it already does enough and if I was going to recommend any of these editors to the publishers I work with, it would be Penflip.