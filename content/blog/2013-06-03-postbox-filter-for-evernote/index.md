+++
title = "Postbox filter for Evernote"
description = "This Postbox message filter organises then sends iTunes receipts to Evernote"
date = 2013-06-03
[taxonomies]
tags = ["apps", "Postbox"]
+++

The Postbox filter described below organises then sends iTunes receipts to Evernote, ready for me to browse when it comes to completing my quarterly VAT return.

I’ve been using note-taking app [Evernote](https://evernote.com) to help manage my financial affairs for a couple of years. For the most part, this has involved storing PDFs for paperless bills and statements. Every quarter when it’s time to complete the dreaded VAT return, I pop open Evernote and check off my statements and bills.

One lot of receipts have been neglected, though, those from iTunes. I often buy apps through the iTunes Store for work purposes. Up till now I’ve used Gmail to file messages from iTunes in a catchall ‘Orders’ category. This leaves them outside my main system, and from time to time charges for apps that are claimable go unrecorded. As I’m basically doing my quarterly accounts when I complete the VAT return, it also means they are not included in my business costs.

[Postbox](http://www.postbox-inc.com) (currently $9.95; available for Mac OS X and Windows) has a built-in send-to-Evernote button. But that involves manual intervention, and I often forget. A message filter, using my private Evernote email sounded like a much better solution.

{{ image(path="postbox-filter-for-evernote.png", caption="Postbox message filter") }}

The filter watches for messages that contain the string ‘Your receipt No.’ in their subject lines, then it performs three actions on any matching messages:

1. The ‘Add Topic’ action adds the message to that group of messages I like to define as ‘Orders’. ‘Topics’ is a Postbox categorising feature; they are not recognised outside the app.
2. So, my second action adds a Gmail label, also ‘Orders’. If I don’t have access to my computer I’ll still be able to find receipts in the Gmail interface.
3. The third action is the main point of this exercise: to get my iTunes bills into Evernote. The action forwards matching messages to my secret Evernote email address – find your secret Evernote email under ‘Settings’ in the web interface – where they are added to my ‘Inbox’. A new note is created for each message. This means I can easily browse the receipts and add any that are relevant to my ‘accounts’ notebook.

I use a number of Postbox message filters to keep my inbox clean and organised. Let me know in comments if you have any useful Postbox message filters to share.