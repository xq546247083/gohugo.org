---
date: 2013-07-01
lastmod: 2015-12-23
menu:
  main:
    parent: content
next: /doc/content/types
notoc: true
prev: /doc/content/front-matter
title: Sections
weight: 30
---

Hugo believes that you organize your content with a purpose. The same structure
that works to organize your source content is used to organize the rendered
site (see [Organization](/doc/content/organization/)). Following this pattern Hugo
uses the top level of your content organization as **the Section**.

The following example site uses two sections, "post" and "quote".

{{< nohighlight >}}.
└── content
    ├── post
    |   ├── firstpost.md       // <- http://1.com/post/firstpost/
    |   ├── happy
    |   |   └── ness.md        // <- http://1.com/post/happy/ness/
    |   └── secondpost.md      // <- http://1.com/post/secondpost/
    └── quote
        ├── first.md           // <- http://1.com/quote/first/
        └── second.md          // <- http://1.com/quote/second/
{{< /nohighlight >}}

## Section Lists

Hugo will automatically create pages for each section root that list all
of the content in that section. See [List Templates](/doc/templates/list/)
for details on customizing the way they appear.

## Sections and Types

By default everything created within a section will use the content type
that matches the section name.

Section defined in the front matter have the same impact.

To change the type of a given piece of content, simply define the type
in the front matter.

If a layout for a given type hasn't been provided, a default type template will
be used instead provided it exists.

