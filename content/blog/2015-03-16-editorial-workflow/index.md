+++
title = "Keep it simple when establishing an editorial workflow"
description = "A straightforward editorial workflow based around Ulysses for Mac and iPad, and 1Writer"
date = 2015-03-16
[taxonomies]
tags = ["apps", "Ulysses"]
+++

Editorial workflows should be simple. Where a team is involved, the simpler the better. Any member of an editorial team should be able to step in and know where others have left off, avoiding delays when another team member is absent, however important that person is to the team. While my workflows do not usually involve others, they adhere to the same principle – simplicity is best.

Projects are separated into two workflows according to type: books and everything else. All projects, regardless of type, are written or edited in a Markdown editor and saved in plain text format. Only if the demands of a particular client requires it is a piece of work output and delivered in an alternative format, such as rich text (.rtf). 

### The book workflow

Manuscripts for books always arrive as MS Word documents. I refuse to buy that unnecessarily sluggish and overweight application, preferring the fast, lightweight, distraction-free nature of a Markdown editor. Pages for Mac, therefore, becomes the middleman between books supplied as MS Word documents and my Markdown editor of choice, Ulysses for Mac ($40). When a book arrives for editing, I open the document in Pages for Mac, Select All (⌘-A), Copy (⌘-C), close the Pages document, open Ulysses for Mac, create a new ‘Group’ in the iCloud section of the sidebar, name it using the book’s title, add a new ‘sheet’ (⌘-N), and paste the entire book into that ‘sheet’.

The next step is to ‘split’ the book into its component parts, or chapters. Working my way through the manuscript in Ulysses, I place the cursor after the book title, the prelims, and individual chapters, and split (Edit \> Split at selection) the document as I go. When I am finished each book part has its own sheet. Then I select all of the sheets and glue (⌘-J) them together. The action of ‘gluing’ comes in handy at the end of a project when I may want to output the book as a single file again, usually in .rtf format, for further processing, or typesetting. The entire process of setting up a book project like this in Ulysses generally takes less than 10 minutes. Editing it takes somewhat longer.

{{ image(path="editorial-workflow-1-588.png", caption="An example book project in Ulysses") }}

The release of Ulysses for iPad ($19.99) last week means I can now work on book projects on my favourite writing and editing device, with everything synced via iCloud. Existing users of Ulysses for Mac will appreciate the iPad app’s similarity to the desktop version, which provides a near-seamless experience and transforms The Soulmen’s flagship software into a go-anywhere app. I will return to discussing Ulysses for iPad later.  

### The ‘everything else’ workflow

When I say ‘everything else’, I mean absolutely everything – articles for print, whether I am writing them or merely editing them, blog posts, general notes, instructional notes, stylesheets, manuals and more. Every piece of writing, amounting to thousands of documents accumulated over the past few years, resides in a single folder. The location of that folder has changed a number of times over the years, but the documents inside it have all stayed together. Currently that ‘folder’ is the one for 1Writer ($2.99) located in iCloud Drive on my Mac. All documents can be accessed using any text editor on my Mac, including Ulysses, where it can be added as an External Source. It is worth noting that when the 1Writer folder is added to Ulysses it returns an item called ‘Documents’, not ‘1Writer’. Don’t ask. Those same documents are then also available to me in 1Writer on my iPad and iPhone. I rarely use the latter, but it is important to have access to those notes wherever I am.

The single folder concept evolved from using Brett Terpstra’s [nvALT](http://brettterpstra.com/projects/nvalt/) – all notes in plain text, all notes in a single folder, all notes accessible anywhere. nvALT serves as a repository on my Mac, reading all notes from the 1Writer folder mentioned above. The only reason it is not the app I use for writing and editing is its lack of syntax highlighting, which is present in most every other Markdown editor I could name, with the exception of Desk, £20.99), a relatively new addition to the Markdown editor fold. 

The secret to keeping all your notes organised in a single folder is a solid naming convention. In the past I wrote about Tyler Reinhard’s [Semantic Notes’](/blog/2013-01-08-getting-things-done-with-semantic-notes) system, which I still use parts of today, but in the interim I have taken on a number of new projects that involve generating numerous additional documents every month. For example, I recently became the editor of a monthly newspaper, *Wrights Farming Register*, wait for it, about farming machinery. As the sole member of the editorial staff, I generate around 80% of the content; the remainder comes from contributors. I process their copy from MS Word documents to my Markdown editor in the same way I do my own. Here is how those files are named:

	wfrx-201504-22-section-name.txt

The first part of the file name, `wfrx`, singles out all documents relating to content for Wrights, the first string of numbers gives me the issue, the second string the page number, and lastly there’s the section name – news or plant and machinery, for example.

When I want to see only those documents relating to the current issue of Wrights, in this case the April issue, I target Ulysses for Mac’s sheet search field (⌘-⇧-F) and type `wfrx-201504` (below – note that this document, unrelated to Wrights, also appears because the body contains that same string of letters and numbers). I can do the same in 1Writer on my iPad to filter out all documents other than those for the current issue of Wrights.

{{ image(path="editorial-workflow-2-588.png", caption="Filtering files in Ulysses. Note the entry in the search field at the bottom of the screenshot") }}
 
The ‘x’ after ‘wfr’ denotes that a document is part of an issue’s content. If I want to filter to all content ever produced for Wrights, I can simply search for ‘wfrx’, thus avoiding administrative notes I have for that publication where the title is often abbreviated as ‘WFR’. Searching in many apps is full depth, which means it returns any document that contains your query, not only those that have it in their file name. Hope that makes sense.

In a similar manner, I prepend filenames for posts to this blog with ‘wdx’, e.g. `wdx-post-title`. I write fewer posts than I would like to, so that simple construction will suffice for now.

### Ulysses or 1Writer?

This post was never intended to be a full review of either app and, in a sense, they are not really competing. Ulysses for Mac is a sound choice, with its ability to organise larger projects, such as books, as well as access external sources. 1Writer is not available for the Mac, but, handily for me, its files are stored in iCloud, which means they can be accessed and edited using other apps, including Ulysses.  

Ulysses for iPad extends the reach and usefulness of its Mac-based sibling for book projects. If I was willing to give up on the idea that my notes should be accessible from everywhere, and from any app, then I dare say Ulysses would do a fine job. But I am not. As things stand, Ulysses for iPad, among many other apps, is limited in its ability to access external files. While it can import files stored in iCloud, such as those created by 1Writer, it can only do so one file at a time, making the importation of thousands of notes a logistical nightmare, and one that would be ongoing, as each new note created externally would have to be imported individually. It is also worth noting at this point that Dropbox support is on Ulysses for iPad’s developers’ roadmap.

For that reason and the fact that it is a solid Markdown editor in its own right, I am happy to store and edit my notes in 1Writer on my iPad. 1Writer also has an internal browser, accessible by swiping left while in any document, a useful research tool.

### Backing it all up

Back up, you say. Aren’t your files already backed up to iCloud? You can never have too many back-ups, I say. On my Mac, I use a simple rule in Noodlesoft’s [Hazel](http://www.noodlesoft.com/hazel.php), a system preference pane, to watch the 1Writer folder in iCloud Drive for new and modified documents and update and sync any changes to third-party storage service Copy. The date in the rule is set as the day before the first note in my collection was created.

{{ image(path="editorial-workflow-3-588.png", caption="A simple rule in Hazel ensures files are automatically backed up and synced with a third-party cloud service") }}

With the introduction of Ulysses for iPad, the developers also took the opportunity to update Ulysses for Mac to version 2.0. The update brings numerous improvements to what was already a great app, a few of which I will mention here. The entire interface has been redesigned to reflect the latest OS X update to Yosemite. Favourite documents now reside in the sidebar, quick export (⌘-6) has been revamped, there is a new dark mode, visible upload and download status for sheets, and attachments – keywords, notes, images – now have their own place on the toolbar. Note, though, that Ulysses’ attachment system for images does not work with external folders.

One thing I would like to see change is the manner in which Ulysses sorts documents. Change the sort status from ‘Manual’ to ‘Date Modified’ and the new status is applied to all projects, not only the active one. After changing the sort configuration, switch from a collection of notes for which the preferred view might be by ‘Date Modified’ to a book project – where a ‘Manual’ sort would be more appropriate – and chapters (sheets) are rendered in reverse order, assuming that project is intended to start with a sheet for the title page and end with a sheet for chapter *n*. Go back and change the sort status if you want to see your book rendered properly. 

That is a small quibble to have with what on the whole is one helluva a Markdown editor.