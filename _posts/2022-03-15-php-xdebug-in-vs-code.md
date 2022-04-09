---
title: 'PHP: XDebug in VS Code'
date: '2022-03-15T08:04:00-04:00'
author: 'Ryan Robinson'
layout: post
permalink: /websites/php-xdebug-in-vs-code/
image:
  src: /assets/img/logo/Visual-Studio-Code.png
  width: 300
  height: 300
  alt: "Visual Studio Code logo"
categories:
  - Websites
tags:
  - PHP
  - 'Visual Studio Code'
---

[XDebug](https://xdebug.org/) is a helpful tool when debugging PHP code. XDebug is a step debugging tools that helps you inspect functionality of PHP code in a cleaner way than regularly writing dump/log statements.

I will not get into details here about setting up XDebug on a server, but you can find that with some Internet searching. Instead, this post is about how to use XDebug within Visual Studio Code.

## Install the Extension

First, install [the extension PHP Debug (xdebug.php-debug) from the Visual Studio Code extension directory](https://marketplace.visualstudio.com/items?itemName=xdebug.php-debug).

!["Visual Studio Code extension page"](/assets/img/2022/03/PHP-Debug-extension-page.png)
_Screenshot of the extension in the directory_

### Start the Listener

To start the XDebug listener:

1. Go to the “Run and Debug” tab (Ctrl + Shift + D) in the main app sidebar.
2. Click the play button beside the XDebug listener. Depending on your developer environment, you may have other listeners as well.

A small window will be added to your workspace with a few buttons. While everything is running smoothly, it will be a pause, a stop, and a restart button. While stopped because of a breakpoint, it will provide other options to continue, step over, step into, and step out.

!["XDebug in VS Code debug panel"](/assets/img/2022/03/Debug-panel.png)
_Debug panel_

### Monitor Notices, Warnings, etc

You can monitor for any notices, warnings, errors, or exceptions that occur while the listener is running.

1. Go to the “Run and Debug” tab (Ctrl + Shift + D) in the main app sidebar.
2. If it is collapsed, expand the “Breakpoints” accordion section.
3. Select under what conditions you want to break and show you results, e.g. Notices, Warnings.

### Add a Breakpoint

You can add a breakpoint at a line in the code and have XDebug report the value of variables as of the start of that line.

1. In the VS Code editor for the code you want to check, scroll to the left of the line of code you want to break. This will cause a little red dot to appear. Click on that red dot to create the breakpoint.
2. Carry out your test scenario (e.g. load the page that calls that PHP in your browser).
3. See the results with the values of each variable at the breakpoint, within the Run and Debug window in VS Code.

!["Visual Studio Code with an XDebug breakpoint set"](/assets/img/2022/03/XDebug-breakpoint.png)
_Breakpoint beside line of PHP code_
