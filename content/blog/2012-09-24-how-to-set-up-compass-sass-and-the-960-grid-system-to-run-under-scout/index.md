+++
title = "How to set up Compass, Sass and the 960 Grid System to run under Scout"
description = "Compass works with Sass to help you write CSS code cleaner and more quickly. Add Scout app for a command-line-free workflow"
date = 2012-09-24
[taxonomies]
tags = ["web design", "Compass", "Sass"]
+++
I don’t spend every day building websites, which is why I lean towards suites of tools that allow me to get things done quicker, and usually without resorting to the command line.

The following method – post installing [Compass](http://compass-style.org/reference/compass/) and the [960 Grid System](https://github.com/nextmat/compass-960-plugin) – steers clear of the command line. Use it to set up a local development environment. The instructions are for Mac users, who will find their command line in Terminal (/Applications/Utilities). Let’s get started.

Open Terminal and type the following after the prompt ($):

`sudo gem install compass`

When asked, type your password and wait a minute or so for Compass to install. If you don’t plan to use the 960 Grid System, you can omit the next step. If you do plan to use it, type the following after Terminal’s prompt:

`sudo gem install compass-960-plugin`

Again, type your password when prompted. When the installation completes, close Terminal and forget about the command line.

Now, download and install <a href="http://mhs.github.com/scout-app/" title="Scout App">Scout</a>.

### Your first Compass project using Scout

At this point, you would normally have to return to the command line and start typing instructions that mean little or nothing to you. But, as you’ve added Scout to your armoury, you don’t have to do that. Find Scout in your Applications folder and double-click to launch. You will be faced with the following window – one that’s so simple, and empty, you could be forgiven for thinking it does nothing at all. But Scout works quietly, and powerfully, in the background, monitoring and updating your projects every time you make a change.
{{ image(path="scout-1.jpg", caption="Scout’s empty interface can be deceptive") }}

Click the plus sign to create your first project. For the purposes of this exercise, in the window that appears switch to your ‘Sites’ folder and create a new folder call ‘Test’. Click ‘Open’ and the Scout interface will now show your first project.

{{ image(path="scout-2.jpg", caption="Scout app showing your first project in the left-hand panel with configuration options on the right") }}

Now tell Scout where to find your project files. Under ‘Stylesheet Directories’, start by choosing an ‘Input Folder’. Click ‘Choose’ and add a new folder to your project called ‘scss’. Do the same for the ‘Output folder’, but this time call it ‘css’. Click the play icon in the left panel. Scout is now monitoring your project, but it won’t do anything till you add something. So let’s remedy that.

Launch your favourite text editor, create a file called ‘style.scss’ and add the following lines. Save style.scss in your project folder inside the ‘scss’ folder you created earlier.

`@import "compass";`
`@import "960/grid";`

`/* Start coding your site below here */`

Your first project is ready to roll. Review the reference section on the Compass website, learn more about Sass on [The Sass Way](http://thesassway.com/beginner) and find out more about using the 960 Grid System Plugin on Github.