---
author: oldadmin
categories:
- Lyricue releases
- Releases
date: "2013-08-20T10:45:03Z"
guid: http://www.lyricue.org/?p=333
id: 333
title: Lyricue 3.6.0 (and 3.6.1) released &#8211; major new features!
url: /2013/08/20/lyricue-3-6-0-and-3-6-1-released-major-new-features/
---

A new version of Lyricue has been pushed to the repository now.  
(3.6.1 was just a quick fix for some database creation issues)

Download the source from [www.lyricue.org/archive/lyricue\_3.6.1.tar.gz](http://www.lyricue.org/archive/lyricue_3.6.1.tar.gz)  
Or install from the PPA – See <https://launchpad.net/~chris-debenham/+archive/lyricue> for details on how to do this

It does bring in some fairly major changes under the hood – but the new features are entirely optional so if you don’t use them nothing should change for you.

The two main changes are the move to using Avahi(zeroconf) to discover displays and the introduction of ‘Profiles’.

There is also the introduction of a ‘simple’ server type. This type of output is designed for the singers/worship team and disables backgrounds to make it less distracting for the musicians.  
The move to using Avahi to find displays means that you can just run up lyricue\_display on a new host and the interface will dynamically find it and start updating it.  
This means that as you add displays they will now show up on the fly on the right of the interface under the ‘Miniview’ section.  
You can then click on individual displays in that section to disable/enable them for updates.  
The result of this is you could have a projector for the congregation (running the normal server) and another one for the worship team (running the simple server) and control them independently.  
For example during an item you could start some nice video playing on the projectors, disable the congregation screen (the video will keep playing) and display the lyrics for the item on the worship team screen.  
This means that the congregation just sees the video (or image or whatever) and the worship team sees the lyrics. Once the item is done you click the congregation preview to re-enable it and continue the service as normal.  
Another use for this functionality would be to have another small computer in an overflow room, or in the creche room, and have it so that it is being updated in sync with the main room.  
The Profiles feature enables you to have a single database storing all the songs – but independent settings and playlists.  
Each host can be associated with a profile or you can change profiles on the fly.  
So you could have a bunch of playlists used for your normal services – and another profile for some other group who also uses Lyricue (such as ‘Mainly Music’)  
Then the two groups can use different images/backgrounds (or the same if desired), different fonts and different playlists.  
Due to the way Lyricue works you can even have two independent profiles running at the same time and they won’t interrupt each other.  
For example you have your main computer running the ‘Default’ profile (and so the projector running from that computer is also on the ‘Default’ profile) and in another room you have a laptop running the ‘Sunday School’ profile.  
The interface running on each one will only affect projectors using the same profile so they won’t get in each others way.

There have also been a few bug fixes (mainly to do with configuration handling – ~/.local/share/lyricue/config2 is no longer used so can’t get corrupted 😉 ) and SQLite support has been removed (it was broken anyway and has been for a while)