# followme-web

Web front end to the companion [followme-android](https://github.com/joshmcarthur/followme-android) project. It is built as a Github Page site and is available at http://joshmcarthur/followme-web

Literally a single HTML file, quickly put together to accept WebRTC data from the Android application. It does the job, but is not particularly versatile or stable. 

Improvements are planned:

* Better handling of missing peer ID
* Error handling for WebRTC messing up
* More information about location - last update time, etc.
* Replacing the marker with something more 'current-location'y, and smoothly animating the marker between points.


SSL
---

I was hoping to make the viewer site available over SSL, however it appears that Peer.js does not support SSL on it's cloud service. Until such time as I can deloy my own Peer.js server to broker RTC connections, the viewer will only work without HTTPS.