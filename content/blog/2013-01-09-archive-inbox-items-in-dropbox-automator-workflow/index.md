+++
title = "Archive your Semantic Notes in Dropbox using this easy to create Automator workflow"
description = "An Automator iCal workflow for backing up and renaming files automatically. Get things done. Look, no hands!"
date = 2013-01-09
[taxonomies]
tags = ["productivity", "Automator"]
+++

After reading Tyler Reinhard’s [Getting Things Done with Semantic Notes](http://semanot.es) a couple of days ago, I was keen to start implementing the system immediately. While I wouldn’t describe my note-taking system as chaotic, it certainly isn’t GTD friendly.

One of the keys to making the system work properly is a solid approach to archiving. Reinhard recommends [Hazel](http://www.noodlesoft.com/hazel.php), an app that allows you to create rules to keep your files organised, among other things. Right now, that’s a problem; my app budget is exhausted. I figured there must be a way to do something similar using Mac OS X’s built-in Automator app. Turns out there is.

According to Reinhard’s system, you export files that are ready for archiving from nvALT to your site-wide ‘Inbox’. Instead of calling on Hazel, the following Automator workflow does the rest:

* Grabs any files you’ve added to the ‘Inbox’
* Renames the files by adding the current date (see the dropdown for other options)
* Moves the renamed files to your Notes Archive folder in [Dropbox](http://db.tt/jw9tyCz).

Let’s get started. It won’t take long. Launch Automator, select ‘Calendar Alarm’ and click ‘Choose’.

{{ image(path="automator-SN1.jpg", caption="Automator") }}

Now you need to add some ‘Actions’ to build your workflow. I find clicking ‘Library’ in the leftmost panel and typing a few letters in the Automator search bar is the quickest way to find specific actions. Locate each of following actions and drag them into your workflow. It’s important that you add them in the order they are shown:

* **Get Specified Finder Items**
* **Get Folder Contents**
* **Rename Finder Items**: click ‘Don’t add’ when prompted to add a Copy Finder Items action. Note that in the screenshot below this action is labelled ‘Add Date or Time’.
*   **Move Finder Items**.

{{ image(path="automator-SN2.jpg", caption="Automator") }}

Three of the actions need further input:

* **Get Specified Finder Items**: Drag your Inbox folder onto this action to add it.
* **Rename Finder Items**: Adjust the dropdowns to your liking. For the record, Reinhard’s Semantic Notes system recommends adding the current date at the end of the filename.
* **Move Finder Items**: Drag your archive folder onto this action to add it.

{{ image(path="automator-SN3.jpg", caption="Automator") }}

Finished? Choose save and give your iCal workflow a name. In reality I opted for the catchy ‘Archive Inbox Items to Notes Archive’; for this post I’ve created one called ‘Test of iCal Alarm Workflow’. Snappy, eh? Onwards, iCal will open and your workflow will appear as an alarm set for the current date and time. Ignore the other alarms showing in the calendar, below. The one we’re interested in is highlighted as ‘Today, 9 January: Test of iCal Alarm…’

{{ image(path="automator-SN4.jpg", caption="Automator") }}

Alter the time and repeats to suit. If you think a weekly backup is enough for your needs, go ahead; I’ve set my workflow to run twice a day: at 6pm (to archive any notes exported during my working day); and at 7am (to catch any notes exported to my inbox after working hours the night before). To run the workflow more than once:

* ⌘N to create a new event; give it a name and hit return.
* Set date, repeat and time to suit.
* Two-third’s of the way down, click ‘None’ and select ‘Open file’. More options are revealed.
* Click ‘iCal’ and select ‘Other’ to locate your workflow file. You’ll find it under /Users/Username/Library/Workflows/Applications/Calendar/.
* Click ‘Done’.

You’re done!

The key difference between this workflow and the Hazel rule Reinhard proposes is that Hazel will watch your inbox and execute the backup procedure as soon as a new document is added. It’s instant.

I don’t doubt there are other ways to achieve the same results as the Automator workflow I describe here, including Applescript.