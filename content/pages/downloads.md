---
title: Downloads
date: '2009-07-28T18:31:35+10:00'
author: cjd
layout: page
menu:
  main:
    name: Downloads
    weight: 10
---

**Lyricue**

**Current Version: *3.4.10***

The easiest way to download/install is using the [PPA repository](https://launchpad.net/%7Echris-debenham/+archive/lyricue) for Ubuntu  
To do this open a terminal and run the following commands.  
`<br></br>sudo apt-add-repository ppa:chris-debenham/lyricue<br></br>sudo apt-get update<br></br>sudo apt-get install lyricue<br></br>`

If you are not running Ubuntu then choose the release series that is the closest match to your system or install from source

- Source package: [lyricue\_3.4.10.orig.tar.gz](/archive)

**Lyricue Remote for Android**

[  
 ![Get it on Google Play](http://www.android.com/images/brand/get_it_on_play_logo_large.png)  ](http://play.google.com/store/apps/details?id=org.lyricue.android)

**Precue**

**Current Version: 1.10**

The easiest way to download/install is using the [PPA repository](https://launchpad.net/%7Echris-debenham/+archive/lyricue) for Ubuntu  
To do this open a terminal and run the following commands.  
`<br></br>sudo apt-add-repository ppa:chris-debenham/lyricue<br></br>sudo apt-get update<br></br>sudo apt-get install precue<br></br>`

See https://launchpad.net/~chris-debenham/+archive/lyricue for details on how to do this.

If you are not running Ubuntu then choose the release series that is the closest match to your system

You can also download the package by itself in various forms:

- Tarball package:[precue\_1.10.tar.gz](/archive)

To install the tarball extract it into a directory on your webserver.

If the webserver is not the same machine as the lyricue database edit session.php and change the $db\_host variable to your lyricue server hostname

**Song Downloads**

Lyricue can load songs from a number of formats but it’s native format is a custom xml file which has been compressed

To install just download a suitable .xmlz file from below and then choose ‘Import Songlist’ from the File menu.

This will bring up a dialog from where you can choose the downloaded file.

Once the file is opened you will be presented with a list of the songs in the file and you can choose which to import or not import

- [English samples – 780 songs (168K filesize)](/songlists/english-samples.xmlz)
- [Deutsch/German samples – 31 songs (8K filesize)](/songlists/deutsch-samples.xmlz)

Note: The usage/display of these songs may be dependant on the copyright laws in your area. They are provided here only as an aid for users. Check your local laws if concerned.

**Bible Downloads**

Lyricue can load bible verses from either via it’s own SQL format, or any sword bible module

### Sword Format

Lyricue can use bible translations from the Sword project as long as you have a small utility called ‘diatheke’ installed. If diatheke is installed any sword bibles installed will show up automatically without configuration. You may need to add/install the ‘diatheke’ tool from your package manager

Sword bibles are also used by [Bibletime](http://www.bibletime.info) and [Gnomesword/Xiphos](http://xiphos.org)

The most common method is to download from [Crosswire.org](http://crosswire.org/sword/modules/ModDisp.jsp?modType=Bibles).

The Sword project provides a number of bible translations in a number of different languages. When downloading from there please use the ‘Raw ZIP’ download.

Your distribution may also provide pre-made packages for some bible texts.

In the case of [Ubuntu](http://packages.ubuntu.com/search?keywords=sword-text&searchon=names&suite=karmic&section=all) and [Debian](http://packages.debian.org/search?keywords=sword-text&searchon=names&suite=stable&section=all) the packages are named ‘sword-text-\*’. On other distributions they may be named differently.

### Lyricue Database Format

Lyricue can import bibles in it’s own SQL-based format.

- [MySQL\_create\_bible\_KJV.sql.gz](/bible_files/MySQL_create_bible_KJV.sql.gz) – King James Version
- [MySQL\_create\_bible\_MES.sql.gz](/bible_files/MySQL_create_bible_MES.sql.gz) – The Message
- [MySQL\_create\_bible\_NIV.sql.gz](/bible_files/MySQL_create_bible_NIV.sql.gz) – New International Version
- [MySQL\_create\_bible\_NIV\_uk.sql.gz](/bible_files/MySQL_create_bible_NIV_uk.sql.gz) – New Internation Version – UK English
- [MySQL\_create\_bible\_NIRV.sql.gz](/bible_files/MySQL_create_bible_NIRV.sql.gz) – New International Readers Version
- [MySQL\_create\_bible\_NLT.sql.gz](/bible_files/MySQL_create_bible_NLT.sql.gz) – New Living Translation
- [MySQL\_create\_bible\_NRSV.sql.gz](/bible_files/MySQL_create_bible_NRSV.sql.gz) – New Revised Standard Version
- [MySQL\_create\_bible\_GNT.sql.gz](/bible_files/MySQL_create_bible_GNT.sql.gz) – Good News Translation
- [MySQL\_create\_bible\_NASB.sql.gz](/bible_files/MySQL_create_bible_NASB.sql.gz) – New American Standard Bible
- [MySQL\_create\_bible\_CJB\_v01.sql.gz](/bible_files/MySQL_create_bible_CJB_v01.sql.gz) – Complete Jewish Bible

## Installation

### Installation from within Lyricue

To use select “Install New Bibles” from the “Bible” menu. From there you can import a Lyricue SQL format or Sword format bible that you have previously downloaded \[img\_assist|nid=47|title=Import bible dialog|desc=|link=none|align=center|width=448|height=278\]

### How to install Sword format automatically

Your distribution may also provide pre-made packages for some bible texts.

In the case of [Ubuntu](http://packages.ubuntu.com/search?keywords=sword-text&searchon=names&suite=jaunty&section=all) and [Debian](http://packages.debian.org/search?keywords=sword-text&searchon=names&suite=stable&section=all) the packages are named ‘sword-text-\*’. On other distributions they may be named differently. Install using your distributions usual package manager. You will also need to ensure that the ‘diatheke’ package is installed.

### How to install SQL format Manually

To install a bible translation download one of the files listed below and then run `gzip -dc bible.sql.gz | mysql -uroot -p` Replace `bible.sql.gz` with the file you downloaded previously.

This should ask for your mysql root user password then install the bible. The next time you run lyricue it will be in the list of available bibles. If your MySQL install does not require a password for the root user remove the `-p` from the command above.

### How to install Sword format Manually

To install a sword format manually run `unzip bible.zip -d ~/.sword`

Replace `bible.zip` with the file you downloaded previously. You will also need to ensure that the ‘diatheke’ utility is installed.
