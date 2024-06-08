+++
title = "Use Hazel with ImageOptim to automate your image-processing workflow"
description = "Optimising images for the web can be a time-consuming task. Here, I hand off part of my workflow to Mac utility Hazel and compression software ImageOptim"
date = 2013-06-17
[taxonomies]
tags = ["apps", "productivity"]
+++

All images uploaded to this site are compressed in [ImageOptim](http://imageoptim.com) – free, open-source software for the Mac – after being put through Photoshop’s ‘Save for web’ routine. But I decided some time ago that that part of my workflow could be speeded up by using [Hazel](http://www.noodlesoft.com/hazel.php), a handy little utility for the Mac.

### Let Hazel do the heavylifting

When I’ve finished adjusting images in Photoshop, which usually involves little more than resizing (and adding a drop shadow in the case of screenshots) – I save them to a folder called **wordius-optimise-me**; in the save dialog, I add a string to the filename, **–600**. This describes the image’s width in pixels – a visual reminder for me more than anything else – and acts as a marker for the simple Hazel rule I use to automate the next stage in my image processing workflow. The Hazel rule is shown in the image below.

{{ image(path="image-optim-hazel-600-io.jpg", caption="Hazel rule for processing images in ImageOptim prior to uploading to this site") }}

The rule tells Hazel to watch for files whose name ends in **–600** in the **wordius-optimise-me** folder. When Hazel encounters images that match this rule, it opens them in ImageOptim (screenshot below), renames each by adding **-io** to the filename – a flag that tells me images have been ImageOptim(ised) – and moves them to another folder, **wordius-web-optimised**, otherwise known as my upload folder.

{{ image(path="image-optim-600-io.jpg", caption="The ImageOptim window tells you which images have been processed, the file size and how much the app’s compression parameters have saved over the original file size") }}

That’s all there is to it.

### But what if you don’t have Hazel?

Well, you could simply drag and drop images onto the ImageOptim application window. But there is another way. Jamie Mason’s [ImageOptim-CLI](https://github.com/JamieMason/ImageOptim-CLI), brought to my attention yesterday by @SmashingMag, automates batch processing of images with ImageOptim, [ImageAlpha](http://pngmini.com/) and [JPEGmini for Mac](http://jpegmini.com/mac) to make lossless optimisation of images part of an automated build process.

Writing this post reminded that there are lots of other areas of my image processing workflow that need automating. I think I’ll start by creating a Photoshop action to capture all the processing steps I repeat every time I prepare an image for this site. Maybe there’s an end-to-end workflow in there somewhere, starting with an original being opened in Photoshop and ending with a file ready to be uploaded to this site. We’ll see.