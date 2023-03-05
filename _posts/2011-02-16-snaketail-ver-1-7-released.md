---
title: 'Snaketail ver. 1.7.1 Released'
date: '2012-09-25T01:01:01+01:00'
status: publish
permalink: /2012/snaketail-ver-1-7-released/
author: Snakefoot
excerpt: 'Snaketail ver. 1.7.1 Released'
type: post
---
SnakeTail ver. 1.7.1 is now available, and introduces some enhancements to the user interface:

- Added Most Recent Used (MRU) list of files, that allows one to quickly reopen files
- Added highlight of windows tabs using icons, when file changes are detected (Display tab icon on file change)
- Added option to apply view configuration to all open views (Apply View Options to All)
- Added option to display the current file name in windows tab, when using rolling regex filename (Title match filename)
- Added tooltip to windows tabs, that displays full file path
- Display currently open session name in main window title

I have now also created MSI installer packages, so I could  play a little with Windows Installer XML (WIX) technology.
 Their project templates and “How to”-guides are not very helpful, but luckily there is a lot of documentation on stackoverflow.com.

I probably have to redo the entire user interface sooner or later, to support the Metro Modern User Interface.
Making lots of tiles, Removing all contrast between visual elements. Ensure everything is shown with capital letters.
Optimized for the perfect touch experience, as Microsoft has done with Visual Studio 2012.