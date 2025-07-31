## iPod shuffle Database Builder

This was originally by Martin Fiedler, written maybe twenty years ago for use with Python 2.  The old Python 2 version is still available in his [SourceForge repo](http://shuffle-db.sourceforge.net).  Python 2 is getting very difficult to find in modern Linux distributions, and it seems apprppriate for somebody to do something to bring this software into the modern age.  

The current code is a naive port of what was originally there, adjusted for linguistic differences to the extent necessary to make it function (I think) correctly on a current system, but it may eventually see future enhancements and bug fixes or even partial rewrites.  The initial version is basically the last release of Martin's program, v1.0-rc1 without any enhancements, but it's different enough that you should consider it to be the start of a new fork, in an earlier stage of development.

###To the point:

This is a Python script that can rebuild the database certain iPod shuffles without iTunes or any Apple software.  It requires Python 3 on the host system and not much more.  It also allows you to keep whatever directory structure you like for your music library instead of packing all your files into directories with nonsensical names and no strategy of organization.

This software works *only* on first and second generation shuffles.  If you have a newer player, consider looking at [https://github.com/nims11/IPod-Shuffle-4g](Nimesh Ghelani's similar script) .

###Usage:
This is the easy part:

   1. Copy *3build_db.py* to the root directory of your iPod shuffle
   1. Run it.

The software should now crawl the filesystem on the device and index the music in the database.  It works for me, but the new port especially is not yet well-tested.  It may well break something which requires an iPod to be reset.  **Please do not use this without understanding the risk.**


