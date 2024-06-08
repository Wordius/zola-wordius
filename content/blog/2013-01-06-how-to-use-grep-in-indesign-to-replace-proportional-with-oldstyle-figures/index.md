+++
title = "How to use GREP in InDesign to replace proportional with oldstyle figures"
description = "InDesign’s find/change dialog is a powerful tool that can be used to apply different fonts to regular expressions, such as all digits"
date = 2013-01-06
[taxonomies]
tags = ["Typography", "GREP", "InDesign"]
+++

One of my clients uses a font that only includes the proportional figure style, but prefers figures in text to display as oldstyle. In order to achieve this I have to deploy a second font, a small-caps version.

This creates a problem for me during typesetting, in particular because that client’s market reports can be extremely data heavy. To give you an idea of how data heavy, it is not uncommon for a single digit – 1, say – to appear as many as 70,000 times in a single report. Using find/change to replace just one of the ten digits can take an age; and while InDesign is doing this, it’s consuming a lot of processing power.

Fortunately, there is a better way. It’s called [grep](http://en.wikipedia.org/wiki/Grep). Grep is a utility for searching plain-text data sets for lines matching a regular expression. Even more fortunate is that InDesign has GREP, as Adobe calls it, built in to its find/change dialog. Adobe [describes GREP](http://help.adobe.com/en_US/indesign/cs/using/WSFB3603CC-8D84-48d8-9F77-F3E0644CB0B6a.html) as:

> Advanced, pattern-based search techniques to search for and replace text and formatting.

That all sounds very complex – to me, at least – but the solution is simple.

{{ image(path="indesign-grep-smallcaps.jpg", caption="InDesign’s find/change window with GREP in use") }}

First, select all your text and apply your main body style. Then follow these simple steps:

1. Create a character style in InDesign that will apply your ‘small-caps’ font to selected text.
2. Make sure your cursor is inside the InDesign ‘story’ that contains the text where you want to apply your new character style.
3. Open InDesign’s find/change dialog, ⌘F or select find/change from the edit menu.
4. Select GREP (highlighted in grey in the image below).
5. Under ‘Find what’ type `\d`. In GREP-speak, `\d` stands for ‘any digit’. Leave ‘Change to’ blank.
6. Make sure the ‘Search’ dropdown is set to ‘Story’.
7. Leave ‘Find Format’ blank.
8. Click the ‘Specify attributes to change’ icon, the magnifying glass, to the right of the ‘Change Format’ box.
9. In the dialog that appears select your new character style from the appropriate dropdown and click `OK`.
10. Back in the ‘Find/Change’ dialog your chosen character style should appear in the ‘Change Format’ box. Click `Change all`.

You’ll notice at the top of the find/change dialog that I have saved this find/change action as a query. In full it reads ‘Change all digits to small caps’. Saving a find/change query like this makes it available application-wide, ready to be reused in all future documents.

### Hold on, wouldn’t a nested style be a better solution?

On the face of it, using a GREP nested style within your main body style is the easiest solution, and it may well work for short documents. Unfortunately, it’s impractical when it comes to the 40,000- to 200,000-word documents I have to deal with. Every time you make a change that causes text to reflow, InDesign has to locate and re-apply your nested style later in the document. The delay while InDesign does this is significant, leaving you enough time to make a coffee between edits. In other words, it’s not very practical.
