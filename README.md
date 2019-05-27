# hideforumthreads

This is a userscript I wrote for browsing the popular forum Resetera.com.  It was originally written for a different forum.  Both forums receive, or did receive, a lot of traffic.  So if you'd go to browse threads in the off-topic section, you could see a lot of different threads rotate through the front page over the course of a given day.  There was also the tendency to post a lot of threads about the same types of topics.  I used the forum as a source of general news, since the off-topic section was quite good for that, and I always wanted a way of filtering the threads I saw so that I wouldn't see anything that I knew I wouldn't be interested in.

That's where this script comes in.  It adds controls to the forum pages for hiding threads instantly, as well as setting keywords for ignoring threads which have those keywords in their titles.  The keyword hide feature is especially useful since you only have to enter the keyword once, and all threads related to that topic will disappear, as long as you've chosen your keyword carefully.  The script also supports wildcards as well as full regular expressions for keyword entry, so you can be very specific.

All this makes for a much more satisfying browsing experience, especially since the script is set to automatically fetch more threads from subsequent forum pages to replace the threads that were hidden and still provide you with a full page worth of threads.

Over the years since I've written it, this script has proven very popular amongst other users and I've been supporting it for nearly five years now.  It was a very satisfying experience to finally implement a feature I'd always wanted to see implemented.  I also had a cloud-save feature which saved your keyword and hidden thread settings to a MongoDB store via EC2 automatically, but I had to remove it since my free AWS trial expired.

Since this is a script that will be running inside a browser extension, I just put all the code into one file.  I kept the ES6+ syntax usage to a minimum, and my only outside dependencies are jQuery and jQuery UI references.
