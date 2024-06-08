+++
title = "Put the hex on Mac OS X’s Color Picker"
description = "How to access OS X’s Color Picker in apps where it’s not available by default, and make it more web-design friendly with some hexadecimal goodness"
date = 2013-03-24
[taxonomies]
tags = ["apps", "color picker"]
+++

Among the many things I discovered this morning was that my default browser, Safari, doesn’t allow direct access to OS X’s Color Picker. A quick search also revealed a surprising lack of colour-picker extensions for Safari. What’s more, Color Picker doesn’t do hex colours.

The following solution is a bit of a compromise. It doesn’t provide direct access to Color Picker through Safari, but it does speed up access to OS X’s colour utility. That done, we give Color Picker a hex capability.

### Quicker access to Color Picker

But first let’s promote the Color Picker utility to application status. Thanks to [an old Gigaom post](http://gigaom.com/2009/08/04/os-x-tips-taking-charge-of-the-color-picker/) by Christopher Ryan, that’s easy. Ryan uses AppleScript (Applications > Utilities) to turn Color Picker into an application.

Launch AppleScript and type the following in the editor pane:

    choose color   

Save (⌘S) the ‘script’ in your Applications folder, making sure to choose ‘Application’ from the file format dropdown. That’s it, now you can launch Color Picker as you would any other application.

Okay, let’s juice up Color Picker by giving it the capability to ‘pick’ hex colours.

### Hex up Color Picker

The original Color Picker, below, is great for storing colours and using them between applications. But it doesn’t do hexadecimal colours.

{{ image(path="color-picker-original.jpg", caption="Color Picker original") }}

Let’s rectify that with a little piece of freeware from Rubicode, [RCWebColorPicker](http://rubicode.com/Software/RCWebColorPicker/). Download the Mac OS X 10.x (Universal) version and follow the simple instructions in the readme file to install the colour picker.

Here’s the result.

{{ image(path="color-picker-hex.jpg", caption="Color Picker with hexadecimal values") }}

Now you have quicker access to Color Picker – in apps where it’s not available by default – as well as the ability to pick hexadecimal colours while retaining Safari as your default browser. Of course, you could always make Google Chrome your default browser, but that would be too easy.