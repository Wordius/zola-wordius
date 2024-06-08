+++
title = "Rems, ems or pixels?"
description = "It’s quite possible to use rems, ems and pixels in your CSS all at once, but let’s not be greedy"
date = 2013-01-25
[taxonomies]
tags = ["web design"]
+++

Ever since reading Ethan Marcotte’s [Sizing the legible letter](href="http://blog.typekit.com/2011/11/09/type-study-sizing-the-legible-letter/) in 2011, I’ve been taken by the `rem` as a proportional unit for measuring the size of type. For far longer, I was against using the `em`, the compounding proportional unit that resets the baseline every time the context changes. But I’m a control freak when it comes to type sizing. Before, and through, 2011 I used the pixel unit, and only the pixel, in all its fixed, stubbornly unmoving glory.

For the record, I also used fixed-width layouts; that’s how stuck in the sand my head was. No fluidity here, sir; none at all. The tide is well and truly out.

But after reading Marcotte’s piece I was smitten by the rem’s single-context usage: ‘sizing text up or down from a baseline value’. Make that baseline 10px:

```css
    html {
        font-size: 62.5%;
    } /* 0.625 x 16px = 10px */
```
where 16px is the default browser font-size for [medium text](http://clagnut.com/blog/348/), and you’re talking math for dummies.

It sounded like a no-brainer, so from that day to this I’ve used the rem with a pixel fallback, the latter providing support for IE8 and earlier, and Opera.

### The em has legs

That takes care of font-size. But what about other attributes, such as margins and padding? In ‘On ems and rems’[^3], Filament Group’s Scott Jehl says ‘rems and ems serve different purposes and need not be mutually exclusive’.

He adds:

> [R]ems…can be less helpful when designing proportional whitespace, such as padding and margins that surround the typography in a fluid layout. This is where em units shine. Take for example, a block of content that contains a heading and a paragraph. The amount of spacing that feels comfortable between the heading and the paragraph (and the space between them and adjacent pieces of content) will often change depending on the size of the text. Using em units for the margins and padding in cases like this mean the spacing will automatically adjust in proportion to the font-size, regardless of what it may be.

So, it would seem, the em still has its uses, just not here.

### Still in em denial

This site is what you might call minimally fluid, or adaptive–responsive. The type measure on the main blog element is managed down. In fact, through the first breakpoint at 767px the width of the main body text doesn’t change at all; only the margins contract. It remains fixed at 556px till comfortably below the ‘small tablet’ portrait screen width of 600px. At that point, all restrictions are lifted and fluidity reigns; the tide is in, folks.

All this is achieved using my favoured rem–pixel–fallback formula. Happily these days, though, I write all the code in a CSS preprocessor, [Sass](http://sass-lang.com), which takes care of all the donkey work – the math; yes, even the stuff for dummies. There’s still no place here for the em.

I’m in the process of converting all units for font sizes, paddings, margins and widths to rems. Ray Brown’s [rem()](https://github.com/bitmanic/rem/tree/master/test) Sass mixin is making my life easier. For example, writing this

```css
    .element {
        @include rem('max-width', 556px);
    }
```

in my Sass document translates to

```css
    .element {
        max-width: 556px; // for older browsers
        max-width: 55.6rem; // for funky browsers
    }
```

in my CSS, excluding the comments. So far so good. The mixin is playing ball. You can pick up the full code from github via the link below.

The rem is supported by the current versions of all major browsers, with legacy support in [some](http://caniuse.com/#feat=rem) – not in IE8, mind.