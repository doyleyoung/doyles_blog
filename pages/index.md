Postman <time datetime="2013-07-15" pubday>July 15th 2013</time>
-------

[Postman](http://getpostman.com/) is my new favorite REST web service testing
client.  It installs as a Chrome plugin and allows you to easily create a valid
request.  Each request is saved and you can categorize your requests into
collections.  It's also has a very well done interface that will format
responses for you.  As if that wasn't enough, it's also open source and
available on [GitHub](https://github.com/a85/POSTMan-Chrome-Extension/).  It
will be part of my tool box for a long time to come.

FreeNAS <time datetime="2013-07-09" pubday>July 9th 2013</time>
-------

I have been very happy with my [FreeNAS](http://www.freenas.org) system and just
updated it to the latest release.  It had been a while since I updated and they
have added a plugin system based on BSD jails.  I installed a couple plugins
and they have made they system more useful on my home network.
[MiniDLNA](http://sourceforge.net/projects/freenas/files/FreeNAS-8.3.1/RELEASE-p2/x64/plugins/minidlna-1.0.24_1-amd64.pbi/download)
is great for getting media on my PS3.
[Transmission](http://sourceforge.net/projects/freenas/files/FreeNAS-8.3.1/RELEASE-p2/x64/plugins/transmission-2.77-amd64.pbi/download)
makes torrent downloads available on the system they eventually end up on
anyway.  I have recommended FreeNAS for a while, but these plugins make the
system more useful and much more attractive for a personal development project.
I will definitely be
[writing my own](http://doc.freenas.org/index.php/Creating_your_own_FreeNAS%C2%AE_PBIs)
module when I find an itch I need to scratch.

R Statistical Computing <time datetime="2013-05-31" pubdate>May 31st 2013</time>
-----------------------

While looking for a tool to analyze a large number of test results, I came
across [R](http://www.r-project.org/).  Since I had read about it multiple times
in the past, I decided to give it a shot.  So far it has save me from writing a
number of one-off scripts and I have barely scratched the surface.  For
instance, given a file containing transaction timings this produces mean,
median, max and standard deviation:

```
cat trans_times.log | Rscript -e 'summary (as.numeric (readLines ("stdin")))'
```

Coincidentally, I was looking for a new [Coursera](https://www.coursera.org/)
course and came across the
[Computing for Data Analysis](https://www.coursera.org/course/compdata) course
being offered by [Johns Hopkins University](http://www.jhu.edu/). Sometimes you
just trip over exactly what you need.

JavaScript Ninja <time datetime="2013-05-10" pubdate>May 10th 2013</time>
----------------

I finished reading [Secrets of the JavaScript Ninja](http://jsninja.com/)
last night.  I enjoyed the book's general approach of introducing a topic,
proving how it works (using a testing methodology developed in an example) and
then building upon each topic after it is completely understood.  It also has
the best written and most complete description of JavaScript's scoping I have
ever read.  For a programming book, it was an entertaining read and it has
earned itself a spot on my quick reference book shelf.  I would definitely
recommend it for anyone interested in taking their JavaScript development skills
to the next level.

Mobile Action <time datetime="2013-05-06" pubdate>May 6th 2013</time>
-------------

Today was fairly active for me in the mobile app space.  I found a new game
[Plague Inc](https://play.google.com/store/apps/details?id=com.miniclip.plagueinc),
a new Android developer tools demo app
[DevAppsDirect](https://play.google.com/store/apps/details?id=com.inappsquared.devappsdirect)
and an update of my iOS app
[DayToDay](https://itunes.apple.com/WebObjects/MZStore.woa/wa/viewSoftware?id=596623324&mt=8)
was released.  Plague Inc has a unique game dynamic where you take the role of a
pathogen and your goal is to kill everyone on Earth as quickly and efficiently
as possible.  I've played a couple games and enjoyed it enough to pay the $1.06
for a full unlock.  DevAppsDirect has demos of various
[AOSP](http://source.android.com/) and third party open source modules/libraries.
It is in beta but is already useful if you need to get a feel for what a piece
of code will look like on real hardware.  Finally, the little app I made for my
wife, DayToDay, had an update approved for release on the iOS App Store.  The
update contains a data entry bug fix and some new promotional images.  I was a
bit concerned that the store is showing my retina and standard images together
in one big set when viewed on my iPad mini.  I thought it showed the appropriate
image by device.  Regardless, I won't be releasing an image only update.

The Perl Renaissance <time datetime="2013-05-04" pubdate>May 4th 2013</time>
--------------------

I watched a presentation from [linux.conf.au](http://linux.conf.au/) by Paul
Fenwich (@pjf) titled [The Perl Renaissance](http://lanyrd.com/2013/linuxconfau/szzxt/).
He discussed some of the tools that have brought about the Perl renaissance.
He pointed out a number of the new Perl tools that I have discovered since I
have been writing Perl again: [meta::cpan](https://metacpan.org/),
[perl brew](http://perlbrew.pl/), [cpanm](http://cpanmin.us/),
[Moose](https://metacpan.org/module/Moose).  He also discussed a number of
modules that I have encountered but need to look into further
[Dancer](http://www.perldancer.org/), [Plack](http://plackperl.org/),
[Task::Kensho](https://metacpan.org/module/Task::Kensho).
And finally, he mentioned some tools that I can't wait to use
[Dist::Zilla](https://metacpan.org/module/Dist::Zilla),
[Regexp::Debugger](https://metacpan.org/module/Regexp::Debugger).  This
presentation was definitely worth the time it took to watch and I will
refer to it in the future.

The Grinder and Grinder Analyzer <time datetime="2013-05-02" pubdate>May 2nd 2013</time>
--------------------------------

I have been using [The Grinder](http://grinder.sourceforge.net/) to load test a
network application I am writing at work.  It is easy to set up and does it's
job well.  It also produces useful statistics that I had been converting to csv
and importing into spreadsheets to analyze.  Today, I came across
[Grinder Analyzer](http://track.sourceforge.net/analyzer.html) which parses the
grinder logs and creates nice looking graphs.  Both use Jython which I have a
love/hate relationship with.  I love the Python scripting side, but hate some
of the Java integration (e.g. converting a Jython string to a Java string so I
can call getBytes()).  Overall I consider both valuable additions to my toolset.

Head <time datetime="2013-05-01" pubdate>May 1st 2013</time>
----

I decided I should write about my side projects.  I came up with three good
reasons why this would be beneficial:

1. motivation - writing about my projects makes me want to work on them
1. documentation - side projects can be put aside for long periods
1. ...
1. profit! (sorry)
1. exploration - the blog itself allows me to experiment with technology I am
interested in

After looking at frameworks capable of generating static sites, I decided to go
with [Contenticious](http://memowe.github.io/contenticious/) which is based on
[Mojolicious](http://mojolicio.us).  I recently used
Mojolicious for a work project and really liked it so I used it for my blog.
Also, both are [Perl](http://www.perl.org) based and I just don't write enough
Perl these days.  Not to mention the fact that I went and bought the domain and
I just can't let it go to waste.
