---
title: 'Brandwood A11y Checker'
date: '2023-01-09T08:18:09-05:00'
author: 'Ryan Robinson'
layout: post
permalink: /websites/brandwood-a11y/
categories:
    - 'Websites'
tags:
    - 'Accessibility'
---

Today I learned about an interesting tool: the [Brandwood Accessibility Checker](http://brandwood.com/a11y/). There are lots of tools out there for testing colour contrast and whether it meets the necessary levels to meet accessibility requirements. But in most of those, you enter one colour for the foreground and one for the background and it gives you the contrast ratio and whether that passes.

This one goes a step further and lets you see contrast of text in front of images. This is great for scenarios like a homepage slideshow (slideshows often aren't great for accessibility in other ways, but we'll ignore that for now) where there is text of a title that shows up layered in front of an image. Whether the text is readable with enough contrast might depend on what part of the image the text appears over, so this tool lets you specify your image, your text colour, and lets you move the text around to see what the contrast is against the image at that specific point.

Note that depending on your mobile responsiveness handling and the possibility for other tools like browsers increasing or decreasing the font size, this might still not be a perfect conclusion. The simplest solution when possible is to put the text above or below the image instead of layered on top of it. But if you need to do it, or if you're looking for a tool to help with a more fixed design scenario - like a PDF document or printed poster - this is a nice tool to have in your belt.