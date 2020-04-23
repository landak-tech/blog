# Credits
This side is build using [Jekyll](https://jekyllrb.com/) and themes from [WowThemesNet](https://bootstrapstarter.com/).

# Writing a markdown blog manual
Markdown is a lightweight and easy-to-use syntax for styling all forms of writing on the GitHub platform. This readme willMarkdown is a lightweight and easy-to-use syntax for styling all forms of writing on the GitHub platform. This readme will show you to write a post using Github Markdown Flavour syntax.

## Headings
'# heading 1'
'## heading 2'
'### heading 3'
etc.

## Create links
```
[Yourtextlink] followed by (https://your.url)
```

## Create quote
'> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.'
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## Bold text
```
**bold text**
```
**bold text**

## Italic text
```
*italic text*
```
*italic text*

## Strikethrough
```
~~strikethrough text~~
```
~~strikethrough text~~

## Highlights
```
==highlighted text==
```
==highlighted text==

## Escaped Charaters
```
\*escaped characters\*
```
\*escaped characters\* instead of *escaped characters*

## List
### Unordered
```
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```
* Item 1
* Item 2
  * Item 2a
  * Item 2b
### Ordered
```
1. Item 1
2. Item 2
3. Item 3
   a. Item 3a
   b. Item 3b
```
1. Item 1
2. Item 2
3. Item 3
   a. Item 3a
   b. Item 3b

## Images
![GitHub Logo](/images/logo.png)
```
Format: ![Alt Text](url)
```

## Inline Code
this is your inline `code`.
```
`added code`
```

## Syntax Highlighting
### HTML

```html
<li class="ml-1 mr-1">
    <a target="_blank" href="#">
    <i class="fab fa-twitter"></i>
    </a>
</li>
```

### CSS

```css
.highlight .c {
    color: #999988;
    font-style: italic; 
}
.highlight .err {
    color: #a61717;
    background-color: #e3d2d2; 
}
```

### JS

```js
// alertbar later
$(document).scroll(function () {
    var y = $(this).scrollTop();
    if (y > 280) {
        $('.alertbar').fadeIn();
    } else {
        $('.alertbar').fadeOut();
    }
});
```

### Python

```python
print("Hello World")
```

### Ruby

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

### C

```c
printf("Hello World");
```


## Task List
```
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

## Table
```
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

## Username @mention
Typing an `@` symbol followed by username.

## Paragraphs
You can create a new paragraph by leaving a blank line between lines of text.

## YAML Section
```
---
layout: post
title:  "Inception Movie"
author: john
categories: [ Jekyll, tutorial ]
tags: [red, yellow]
image: assets/images/11.jpg
description: "My review of Inception movie. Acting, plot and something else in this short description."
featured: false
hidden: true
rating: 4.5
beforetoc: 
toc: 
---
```
- `layout:` is to define which layout will be use for this particular page.
- `title:`  will define the title of the page.
- `author:` will define the author of the post, the author setting is in the [_config.yaml](/_config.yml)
- `categories:` will define the caategories of the article.
- `tags`: will define tags related to the article.
- `image:` will define the primary image that will be use for the article.
- `description:` will define the description of the article.
- `featured:` will define if the article will be show on the featured page or not.
- `hidden:` will define if the article will be show on the entire site or not.
- `rating:` create a rating for the article.
- `beforetoc:` create a description that will be shown before the `table of contents`.
- `toc:` create a `table of contents`

## Create Spoiler
```
<span class="spoiler">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span>
```
<span class="spoiler">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</span>

## Full HTML

Perhaps the best part of Markdown is that you're never limited to just Markdown. You can write HTML directly in the Markdown editor and it will just work as HTML usually does. No limits! Here's a standard YouTube embed code as an example:
```html
<p><iframe style="width:100%;" height="315" src="https://www.youtube.com/embed/Cniqsc9QfDo?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe></p>
```
<p><iframe style="width:100%;" height="315" src="https://www.youtube.com/embed/Cniqsc9QfDo?rel=0&amp;showinfo=0" frameborder="0" allowfullscreen></iframe></p>

## Reference lists

The quick brown jumped over the lazy.

Another way to insert links in markdown is using reference lists. You might want to use this style of linking to cite reference material in a Wikipedia-style. All of the links are listed at the end of the document, so you can maintain full separation between content and its source or reference.