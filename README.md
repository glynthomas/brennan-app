# brennan B2 web app archive

brennan releases for the B2 music player, zip files to be saved to a USB stick for upgrading [ rename to b2.tar.gz ] the B2 web app files versions are stored here, together with the last web app release [ dated 11/04/2019 & internal B2 software version Mar 20 2019 12:21:43 ] from brennan

a new updated version & noiseless version branch of this web app, are currently being developed & maintained at http://oksauce.com please visit for more info ...  

# brennan web app noiseless why?

brennan b2 music & radio media player is a great bit of kit and relatively easy to modify, the native web app B2 branch is, i understand no longer being maintained, the web app final release continually polls the b2 unit every half a second for sync & status updates, this polling seems to create the following 'hidden' problems;

-  uploading new music via a network
-  mutiple devices accessing the B2
-  potential radio drop outs
-  performance and browser memory leaks
-  network bandwidth overhead
-  internet issues for other network users

Other small UI issues may need some attention, which are discussed below

# brennan web app noiseless how?

the existing javascript has been tweeked, with functions edited & some added, the constant polling has been removed & replaced with event driven polling, rather than a constant stream of half a second [ 500ms ] network requests!

the new noiseless release implements event polling, which is more like a wave saying hello to the B2 when you access the web app client, leaving the B2 to get on with playing music, radio or uploading files without "noise" problems associated with network polling frequency, where timing is required, a local timer takes over and re-syncs with the B2 when requied [ scrub or time of length of songs ]

# brennan web app update release

a new updated version, based on the [11/04/2019] web app release from brennan is available at http://oksauce.com, this version is fully responsive, with the native mobile view including tone controls, (scrub) time & volume while the dedicated mobile web page has been updated to functioning as designed, available at http://oksauce.com

# brennan web app noiseless release

noiseless web app release is a branch of the latest & last brennan B2 web app UI based on the last release web app [11/04/2019] to focus on just playing music & radio without 'noise' with excellence ... please visit http://oksauce.com for more details

# noiseless release roadmap

major changes include; removal of constant polling of the B2, scrolling graphs and other continued status updates this will remove the problems associated with mutiple devices accessing the B2, music file uploads, radio drop outs and performance and browser memory leak issues created from constant polling to minor fixes which include; removal of hash in the URL and the requirment of an internet connection and a number of other minor performance improvements

UI controls have been tweeked together with improved mobile web UI modal & improved responsive design layout 

## noiseless B2 mobile update

the current official last brennan B2 update offered an experimental mobile only UI, the code base has been recrafted to a noiseless version, the code base has been updated to a fully functional noiseless mobile version, please visit http://oksauce.com for more info
 
official experimental UI is being developed at ... https://github.com/geometryzen/brennan-app 

un-official updated UI & noiseless UI versions are being developed & maintained at http://oksauce.com

###### * please note, all web app upgrades & updates are implemented at your own risk
