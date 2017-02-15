---
layout: post_page
title: JekyllAdventures
---
Footnotes can be added to the body of your text using placeholders like this: [^1]. For example,

This is text with a footnote link at the end. [^1]
Alternatively you can use ‘n’ rather than numbers [^n] so you don’t have to worry about which number you are on. At the very end of your post, you can define your matching footnotes as shown below, URLs will be turned into links:



> Quotes that i really like


***************

Laying down some code with markdown.
*Italics text example*
~~text lined~~
==text highlighted==
**Bold Text!**
So if i wanted to show some code: `code` And then it would be beutiful

![Cat](https://cdn.pixabay.com/photo/2014/03/29/09/17/cat-300572_960_720.jpg)

[Google Link](http://google.com)

*First
*Second
*Third Item

```
<header>
    <h1>{{title}}</h1>
</header>
```
1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |




[^1]: This is my first footnote
[^n]: Visit http://ghost.org
[^n]: A final footnote
