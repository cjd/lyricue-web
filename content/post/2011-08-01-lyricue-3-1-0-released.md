---
author: oldadmin
categories:
- Lyricue releases
date: "2011-08-01T14:26:29Z"
guid: http://www.lyricue.org/2011/08/lyricue-3-1-0-released/
id: 244
title: Lyricue 3.1.0 released
url: /2011/08/01/lyricue-3-1-0-released/
---

 *Mon Aug 1 14:26:27 EST 2011*

After much time I finally decided that lyricue 3.x is at the point I can call it 3.1 🙂  
Since the release of 3.0 a lot of fixes and updates have gone in.  
The main things are:

- Works on Ubuntu oneiric, natty, maverick and lucid
- Handling of non-alpha characters in filenames has been fixed up
- You can associate font/shadow colours with a specific background (with a preview) via the media manager
- Dramatic speed increase in advanced search
- You can press enter to quickly add the first item found when searching the songlist
- Lyricue can directly play DVD titles
- Display live video feed as background
- Online documentation included in the application itself
- Video backgrounds play silently for a few seconds in the preview windows
- Smarter adding of image, video and music files to the playlist
- Imports pptx files (via workaround)
- Better handling of different multi-display setups
- Configuration now stored in the database directly
- Preview window added to edit/add song screen

Lyricue 3.1.0 has the following changes since 3.0.41

- Fix handling of apostrophe in presentation filenames
- Add text overlay in background manager so it is easier to check text colour

Download the source from [www.lyricue.org/archive/lyricue\_3.1.0.tar.gz](http://www.lyricue.org/archive/lyricue_3.1.0.tar.gz)  
Or install from the PPA – See <https://launchpad.net/~chris-debenham/+archive/lyricue> for details on how to do this  
  
Full list of changes since 3.0

- Fix handling of apostrophe in presentation filenames
- Add text overlay in background manager so it is easier to check text colour
- Fix import of images to DB (LP#816937)
- Dramatic speed increase in advanced search (LP#814772)
- Fix handling of semicolons and ampersands in image filenames
- Text/shadow colours should work properly now
- Fix bible changing in preview
- More work on getting text/shadow colour association working with videos
- Fix application menu strings (LP#807237)
- Make DVD playing actually play the selected title
- Add local documentation
- Fix build for maverick/lucid
- Fix audio volume (LP#806715)
- Make pressing enter in available songlist add song to playlist (makes interactive search work)
- Enable videos to play for 3 seconds in miniview
- Make shadow offset actually do something
- Handle symlinks properly when importing a directory
- Allow pressing enter when searching for a song to add first match
- Allow any image, video or music file to be added via ‘add directory’
- Sort list of song when importing
- Fix for importing text songs with unicode
- Fix looping of background videos
- Fix progress bar for videos
- Fix scaling on natty
- Add support for importing pptx (via workaround)
- Initial support for audio files in playlist
- Fix text colour not being updated on re-config
- Fix text colour not being updated
- Fix automatic looping for sublists
- Fixes for Clutter-gst 1.x
- Fix crash when background not specified fully
- Fix video playback related crash (LP#675090)
- Migrate package name from lyricue3 to lyricue
- Hide mouse cursor in display after three seconds of no motion
- Fix video looping for playlist items
- Fix geometry override handling when launching via lyricue
- Default hostname should be ‘localhost’
- Force CLUTTER\_DISABLE\_MIPMAPPED\_TEXT and unset LIBGL\_ALWAYS\_INDIRECT
- lyricue\_display was ignoring database given on commandline
- Lyricue should quote passwords in mysql command (LP#668770)
- Playback control not working (LP#668443)
- Fix handling of &amp; in text display
- Lyricue 3 miniview does not work (LP#640936)
- Cannot use page forward or back when showing an image (LP#665498)
- Work on blank screen behaviour (LP#662311)
- Make ‘OK’ be default action in combo/entry dialogs (LP#665494)
- Add fade/blur effect for backgrounds
- Work on getting aspect ratio displayed right for backgrounds
- Fix Crash when playing videos
- Fix missing break in mouse-click handling (LP#664931)
- Fix lyricue\_display distorts images (LP#664921)
- Fix lyricue\_display ignores font colour setting on songs (LP#664929)
- Add mouse-click handling (LP#664931)
- Fix line-wrap for preview (LP#662893)
- Fix preview window display
- Remove multiple Load/Close Lyricue Display items in menu
- Remove ServerType setting as it is no longer used
- Fix preview in add/edit song dialog
- Increase epoch so will superceed 1:2.3.x
- Don’t complain if access.conf not setup
- Re-add locales
- Don’t complain if access.conf not setup
- Add default items to applications menu to start/stop lyricue\_display
- Add option to lyricue\_remote to close the server
- Set process name for lyricue\_display better
- Turn off debug output by default (use ‘-d’ to re-enable)
- Fix looping not working
- Fix clear-text function
- Fix double-changing of background in preview
- Enable word-wrap by default for songs
- Add lsdvd to dependancies
- Report port number is process name
- Fix crash when going back past first item
- Enable live video backgrounds
- Add .desktop files
- Initial work at dvd support
- Add preview window to edit/add song dialog
- Force writing of config to db every startup (LP#636731)
- Re-add lyricue\_remote command
- Let lyricue\_display use GeometryOverride if set
- Get lyricue\_display to reload config when saving prefs in lyricue
- Implement OSD functionality
- Fix loading lyricue\_display from apps menu
- Save first config to database
- Change some install dependancies
- Make interface work at 1024×600
- Fix status message to return proper screen size
- Fix blank handling after preview
- Fix missing files
- Make presentation import retry if fails
- Store presentation temp files in /var/tmp instead of /tmp
- Packaging changes
- Implement dbimage loading
- Don’t try to set the geometry if it is null
- Make lyricue\_display log to logfile/stderr
- Fixes for bible preview
- Fix crash when blanking screen to database image
- SEMI should be :
- More fixes to preview command
- Change debug messages for verse adding
- Use mipmaps for glyph caches
- Fix preview command
- Fix crash on reconfigure
- Add conflict for lyricue/lyricue-cvs
- Look for sql updates in right directory
- Add sword support