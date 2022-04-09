---
title: 'Drupal: Ckeditor Abbreviation'
date: '2022-03-07T11:35:00-05:00'
author: 'Ryan Robinson'
layout: post
permalink: /websites/drupal/drupal-ckeditor-abbreviation/
image: 
  src: /assets/img/logo/Drupal.png
  width: 300
  height: 300
  alt: "Drupal logo"
categories:
    - Websites
    - Drupal
tags:
    - HTML
---

One of the HTML tags that many are not aware of is [the &lt;abbr&gt; tag](https://www.w3schools.com/TAGS/tag_abbr.asp). This is a useful tag to help provide explanations of abbreviations within the body of the text. If you’re reading along and see an abbreviation for <abbr title="WordPress">WP</abbr> and you know what it is, you can keep reading. If you’re reading along and see an abbreviation and don’t know what it is, you can hover over it and it will show you an explanation. It’s a win-win, providing an explanation for those that need it without needing to add more text in the main body which may come across as over-explaining for those that don’t need it.

To make it easy to insert this tag into Drupal content, you can install [the ckeditor\_abbreviation module](https://www.drupal.org/project/ckeditor_abbreviation). This is a simple but effective module that adds a button to the ckeditor WYSIWYG editing panel that enables users to add an &lt;abbr&gt; without touching any code. The interface fits in seamlessly, with a similar experience to adding a link.
