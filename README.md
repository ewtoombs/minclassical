# minclassical
A minimalist streaming client for Toronto's New Classical FM.

### intro

Toronto's New Classical FM is now hosted online at http://www.classicalfm.ca/.  
Run entirely on javascript, this site is an over-engineered ten tonne 
abomination, deserving of total annihilation. This software maker settled for 
redesign, following reverse engineering. This script is the result. Its 
footprint is small enough to allow it to run on resource-limited systems like 
the Raspberry PI or this software maker's 10-year-old laptop, currently being 
used as a media server.

The basic code can be used on other radio stations on zoomermedia.ca, where 
New Classical is hosted.

### dependencies
1. python 3
1. python websockets
1. python requests
1. mpv (easily exchangeable with other media players.)

### usage
Just run it! :)
```
$ git clone 'https://github.com/ewtoombs/minclassical.git'
$ python minclassical/minclassical
```

### install
Place the script in whichever binary directory you consider appropriate.
```
$ git clone 'https://github.com/ewtoombs/minclassical.git'
$ sudo install --mode=0755 minclassical/minclassical /usr/local/bin.
$ minclassical
```

### more words to read:
But ewtoombs, why didn't you simply use Wireshark or Chrome Developer Tools to 
capture the streaming URL, then save it in a playlist somewhere?

Yes, that is my usual solution to bloated internet radio websites. Much to my 
dismay, though, I discovered that the streaming URLs of this particular radio 
station keep changing, because the IP address is hard coded into the streaming 
URL and there are multiple, possibly-changing IP addresses.  Thus the only way 
to connect reliably to this station is through a script like this.

 vi:fo=atw
