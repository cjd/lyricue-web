---
title: Developers
date: '2009-07-28T21:25:46+10:00'
author: cjd
layout: page
url: /developers
---

If you wish to you can join the lds-devel mailing list (which is for developers) at [lds-devel](http://lists.sourceforge.net/lists/listinfo/lds-devel) or the lds-users mailing list (which is for users 🙂 at [lds-users](http://lists.sourceforge.net/lists/listinfo/lds-users)

Development is done using bazaar inside launchpad so go to <https://code.launchpad.net/lyricue> to view/access/download the current development code

Debian/Ubuntu packages built from bazaar are also available from the apt repository as` lyricue - `see <https://launchpad.net/~chris-debenham/+archive/lyricue>

Bug tracking is handled via Launchpad – see <https://bugs.launchpad.net/lyricue>

To help with translating go to <https://translations.launchpad.net/lyricue>

**Bug tracking**

If you find a bug in Lyricue, or have a suggestion on how to make it better you can log a bug via launchpad at https://bugs.launchpad.net/lyricue

To best assist in determining the problem cause please run the following commands and send the created lyricue\_debug.tgz if requested:

$ mysqldump –skip-compact -ulyric lyricDb &gt; lyricDb.sql

$ tar cvfz lyricue\_debug.tgz lyricDb.sql ~/.local/share/lyricue

To enable extra debugging run lyricue with the ‘-d’ option and capture the terminal output (this will show sql commands run)
