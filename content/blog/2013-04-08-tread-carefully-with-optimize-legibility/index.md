+++
title = "Tread carefully with optimizeLegibility"
description = "optimizeLegibility is useful in some situations, including enabling glyphs in smaller text sizes, but it can produce unexpected results"
date = 2013-04-08
[taxonomies]
tags = ["web design"]
+++

When I’m setting minor headings, I often use `small-caps` on the `font-variant` property. And while I’m at it I add 1px of `letter-spacing` to improve legibility.

It came as a surprise then that the first minor heading I set on this site looked almost acceptable (below), despite the fact I’d forgotten to apply letter-spacing. When I inspected the CSS, I discovered the reason – the `text-rendering` property was being applied to all headings, with a value of ‘optimizeLegibility’.

{{ image(path="optimizeLeg1.jpg", caption="The text-rendering property is set to optimizeLegibility") }}

Unfortunately, another of my minor headings showed less-than-acceptable results – see ‘might’.

{{ image(path="optimizeLeg2.jpg", caption="Whoa! The text-rendering property is set to optimizeLegibility") }}

And when I checked on my iPhone, both headings looked far from optimised. If anything, letter-spacing had been tightened, which made reading them difficult.

Thing is, I didn’t specify the `text-rendering` property in my own CSS. It is applied globally to all headings by the framework I used to build this site, ZURB’s [Foundation](http://foundation.zurb.com). So I went looking for `text-rendering`’s ‘off’ switch to add an override. It seems there isn’t one. There’s no ‘none’ value for `text-rendering`.

After some experimentation, I came up with the following fix:

```css
.section-title {
    text-transform: lowercase;
    font-variant: small-caps;
    text-rendering: auto;
    letter-spacing: 1px;
}
```    
This gives the result I would have expected had `text-rendering` not been applied in the first place, and it’s iOS friendly, too.

{{ image(path="optimizeLeg3.jpg", caption="Better: optimizeLegibility has capitulated; letter-spacing reigns") }}

It’s worth noting that the text-rendering property is not defined in any CSS standard. The [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/CSS/text-rendering) has more.