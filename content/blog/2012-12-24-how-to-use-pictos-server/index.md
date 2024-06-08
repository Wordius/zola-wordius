+++
title = "How to use the Pictos icon fonts server"
description = "This blog uses Pictos icon fonts. Here’s how to get set up"
date = 2012-12-24
[taxonomies]
tags = ["web design", "Pictos"]
+++

_Note: [Mono Social Icons font](http://drinchev.github.io/monosocialiconsfont/) has since replaced Pictos icon fonts on this website._

There are a number of reasons for choosing an icon font over a bitmap image:

* Bitmaps are poor at scaling
* Bitmaps require more http requests
* Bitmaps are difficult to manipulate.

That’s good enough for me. You’ll find a more detailed explanation on Steven Bradley’s Vanseo Design blog in [Why and how to use icon fonts](http://www.vanseodesign.com/web-design/icon-fonts/).

[Font Awesome](http://fortawesome.github.com/Font-Awesome/) has always been my icon font of choice, still is. But when it came to setting up here I was in a rush. I couldn’t find a way to serve the font files to a Scriptogram site, so I turned to Pictos. (I’m still using Pictos, but, after writing this post, I discovered Tim Pietrusky’s [We Love Icon Fonts](http://weloveiconfonts.com/), which he describes as ‘like Google Web Fonts, but icon fonts only’.)

{{ image(path="pictos.jpg", caption="Pictos offers 324 unique interface icons. Image: Pictos") }}

### Set up Pictos Server

[Pictos Server](http://pictos.cc/) allows you to build your own icon font. Here, I’m using the Forever Free plan, as my needs are limited. Features of the plan include:

* No downloadable font purchases 
* Up to 12 icons per font 
* Unlimited fonts 
* 1 domain 
* SSL service.

You can see the font in use in this site’s sidebar – social media and RSS icons – and fronting the post dates. Let’s get to it:

1. Sign up for the Pictos Server Free Plan.
2. Choose up to 12 icons from the ‘Pictos Library’ panel.
3. When an icon you’ve chosen appears in the ‘Chosen Icons’ panel below, assign it a letter of the alphabet. Let logic guide your choice of icon/letter pairings – it may help six months down the line when you decide to make some changes. For instance, I use ‘r’ for the RSS icon and ‘t’ for Twitter.
4. When you’re done selecting, click save and give your font a name. It will appear in the ‘Edit a Combo’ dropdown above the ‘Chosen Icons’ panel.
5. Click ‘Generate code’.
6. Copy the generated code and paste it in the `<head>` of your Scriptogram theme.

### Add Pictos fonts to your code

There are a [number of ways](http://pictos.cc/articles/using-icon-fonts/) to implement Pictos icon fonts; I opted for a simple class:

```css
.pictos {
	font-family: 'Pictos Custom';  
	-webkit-font-smoothing: antialiased;  
}
```
In my HTML, the class is added to an `<i>` tag. As an example, the Twitter logo in this site’s sidebar is generated using the following HTML:

```html
<li>
	<i class="pictos">t </i>
	<a href="http://twitter.com/wordius">Twitter</a>  
</li>
```
And that’s all there is to it.