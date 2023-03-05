---
title: 'SnakeTail'
date: '2011-02-16T01:01:01+01:00'
status: publish
permalink: /snaketail/
author: Snakefoot
excerpt: 'SnakeTail'
type: page
layout: page
---
## SnakeTail ##

SnakeTail is a Windows tail utility for monitoring growing text log files.

- [Download Latest Version](https://github.com/snakefoot/snaketail-net/releases)
- [Report Bugs and Feature Requests](https://github.com/snakefoot/snaketail-net/issues)

Feature list:

- Monitor "large" text log files
- Monitor Windows Event Logs (Without needing administrator rights)
- Multiple Window Modes supported (MDI, Tabbed, Floating)
- Save and load entire window session. Can load session file at startup when given as command line parameter.
- Sentence highlight with colors based on keyword match (Includes regex support)
- Quickly jump between highlighted sentences using keyboard shortcuts
- Toggle bookmarks and quickly jump between bookmarks
- Configure external tools and bind custom shortcut key (Trigger execute on highlight)
- Tails circular logs where the log file is periodically truncated/renamed.
- Tails log directory where the latest log file is displayed (Includes wildcards)
- Search in the entire text log file (Or EventLog)
- Highlight window tabs using icons, when file changes are detected
- Tail new log files with a simple drag drop from Windows Explorer
- Filtering of Windows Event Logs using regular expressions
- Display simple process statistics in window title bar (RAM + CPU usage + TRX/Sec)
- Stop and start Windows service by right clicking in the tail window
- Change tail window background color
- Change tail window text color
- Change tail window icon
- Minimize to tray
- Low memory usage independent of log file size
- Low cpu usage even when more than 100 lines/sec
- Works well over remote desktop
- Supports Windows 2000, XP, 2003, Vista, Win2k8, Win7
- Requires .NET 2.0
- GNU GPL License v3

![SnakeTail with tabs]({{ 'assets/images/snaketail_tabs.png' | relative_url }})
![SnakeTail with dock]({{ 'assets/images/snaketail_mdi.png' | relative_url }})
![SnakeTail with undock]({{ 'assets/images/snaketail_float.png' | relative_url }})

## Version History: ##

#### Ver. 1.9.5 ####

- Add new File-Tab option to open File Explorer in Containing Folder
- Include FileSize in the Windows Title
- Add Open File shortcut (Ctrl+O)

#### Ver. 1.9.4 ####

- Quick jump shortcut has changed to ALT+KeyUp/KeyDown (Instead of CTRL+KeyUp/KeyDown)
- Quick jump also works for EventLog where it jumps between Warnings and Errors
- Toggle application as "Always on top"
- Launch external tools on keyword match (Ex. play sound).
- Line coloring without being ‘Alert highlight’ (Ex. color line green for success)
- Search with wrap-around-support
- Display current file-size in the Windows Title
- Fixed several bugs

#### Ver. 1.8.2 ####

- Added feature to launch external tools, and also bind a custom shortcut key
- Added feature to toggle bookmarks, and quickly jump between bookmarks
- Changed send crash report to perform HTTP upload to www.crash-server.com
- Fixed several bugs

#### Ver. 1.7.1 ####

- Added MSI installer packages

#### Ver. 1.7 ####

- Added Most Recent Used (MRU) list of files, that allows one to quickly reopen files
- Added highlight of windows tabs using icons, when file changes are detected (Display tab icon on file change)
- Added option to apply view configuration to all open views (Apply to All)
- Added option to display the current file name in windows tab, when using rolling regex filename (Title match filename)
- Added tooltip to windows tabs, that displays full file path
- Display currently open session name in main window title
- Fixed several bugs

#### Ver. 1.6 ####

- EventLog can now be searched like a normal text file.
- Fixed several bugs

#### Ver. 1.5.1 ####

- Added keyboard shortcuts for quickly jumping between highlighted lines
- Fixed several bugs

#### Ver. 1.4 ####

- Added reordering of tabs using drag drop
- Added closing of tabs using the middle mouse button
- Added restore of original position for minimized windows, when saving window session
- Added parameter to control how often to check for log file changes (Default every 100 ms)
- Extended command line option to tail arbitrary file (Unless it has .xml as file extension)
- Fixed several bugs with unhandled exceptions.

#### Ver. 1.3 ####

- Added drag drop support for opening new files to tail
- Added support for configuring default configuration when opening new files to tail (Save a session with one configured tail window as ‘SnakeTail.xml’ and place it next to the application)
- Changed ‘Minimize to tray’ so it sticks even if double clicking the tray icon to restore from minimized state.
- Improved handling of circular logs when file is renamed / truncated

#### Ver. 1.2 ####

- Added sentence highlight based on keyword match (Includes regex support)
- Added support for automatic tailing the latest file in folder (Includes regex support)
- Improved error handling when there are problems with tailing a file

#### Ver. 1.1 ####

- Added support for opening multiple files in single operation
- Added support for Check For Updates in the Help menu
- Added support for Send Error Report for unhandled exceptions
- Improved error handling when attempting to open locked files
- Skip runas dialog on Windows XP when stopping/starting service

#### Ver. 1.0 ####

- Extended "Edit"-menu in the main Window to display the context menu of the child window
- Created new View Options-dialog to configure child window options without editing the xml file

#### Ver. 0.9 ####

- Added copy to clipboard for Windows EventLogs
- Fixed copy to clipboard for floating windows
- Fixed scrollbar for floating tail windows

#### Ver. 0.8 ####

- Can now also monitor Windows EventLogs (See "Open EventLog…" in the "File"-menu)
- Can perform filtering on the Windows EventLogs (Right-click in the Event Log window)

#### Ver. 0.7 ####

- Only a single search window, that searches the active tail window
- Can minimize to tray
- Can store free/modeless windows in sessions
- Can monitor admin processes without crashing
- Can override the window icon with something from an external file (IconFile)
- Can monitor how many times a certain text string appears every second (LogHitText)
- Improved detection when applications closes, when run inside a debugger

#### Ver. 0.6 ####

- Fixed saving of font when saving session
- Fixed loosing window title when minimizing just after opening file
- Changed .NET requirement to ver. 2.0
- Added support for display memory and cpu info for normal processes

#### Ver. 0.5 ####

- Command line support to specify session-configuration to load at startup
- Extended session-configuration with servicename
- Can show Service-State, CPU usage and RAM usage for the specified service
- Can stop and start the specified service by right-clicking in the tail window

#### Ver. 0.4 ####

- Support that log file is renamed / deleted and created again
- Session configuration file is now saved in pretty formatted xml.
- Session configuration file now supports relative paths from where the session-file is placed
- Pause / Break key will now stop the active window from scrolling. Press Enter-/Space-key will make it continue
- Alternative one can press page-up several times or use the mouse to scroll up and it will stop scrolling

#### Ver. 0.3 ####

- Progress bar when opening files
- Keeps position at bottom when resizing tail windows
- Improved speed when searching in log windows (and added search progress bar)

#### Ver. 0.2 ####

- Faster startup
- Possible to change text-color