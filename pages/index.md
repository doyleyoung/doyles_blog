Title: Doyle's Blog

Mobile Action <time datetime="2013-05-06" pubdate>May 6th 2013</time>
-------------

Today was fairly active for me in the mobile app space.  I found a new game
[Plague Inc], a new Android developer tools demo app [DevAppsDirect] and an
update of my iOS app [DayToDay] was released.  Plague Inc has a unique game
dynamic where you take the role of a pathogen and your goal is to kill everyone
on Earth as quickly and efficiently as possible.  I've played a couple games and
enjoyed it enough to pay the $1.06 for a full unlock.  DevAppsDirect has demos
of various [AOSP] and third party open source modules/libraries.  It is in beta
but is already useful if you need to get a feel for what a piece of code will
look like on real hardware.  Finally, the little app I made for my wife,
DayToDay, had an update approved for release on the iOS App Store.  The update
contains a data entry bug fix and some new promotional images.  I was a bit
concerned that the store is showing my retina and standard images together in
one big set when viewed on my iPad mini.  I thought it showed the appropriate
image by device.  Regardless, I won't be releasing an image only update.

The Perl Renaissance <time datetime="2013-05-04" pubdate>May 4th 2013</time>
--------------------

I watched a presentation from [linux.conf.au] by Paul Fenwich (@pjf) titled
[The Perl Renaissance].  He discussed some of the tools that have brought about
the Perl renaissance.  He pointed out a number of the new Perl tools that I
have discovered since I have been writing Perl again: [meta::cpan], [perl brew],
[cpanm], [Moose].  He also discussed a number of modules that I have
encountered but need to look into further [Dancer], [Plack], [Task::Kensho].
And finally, he mentioned some tools that I can't wait to use [Dist::Zilla],
[Regexp::Debugger].  This presentation was definitely worth the time it took to
watch and I will definitely refer to it in the future.

The Grinder and Grinder Analyzer <time datetime="2013-05-02" pubdate>May 2nd 2013</time>
--------------------------------

I have been using [The Grinder] to load test a network application I am writing
at work.  It is easy to set up and does it's job well.  It also produces useful
statistics that I had been converting to csv and importing into spreadsheets to
analyze.  Today, I came across [Grinder Analyzer] which parses the grinder logs
and creates nice looking graphs.  Both use Jython which I have a love/hate
relationship with.  I love the Python scripting side, but hate some of the Java
integration (e.g. converting a Jython string to a Java string so I can call
getBytes()).  Overall I consider both valuable additions to my toolset.

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
with [Contenticious] which is based on [Mojolicious].  I recently used
Mojolicious for a work project and really liked it so I used it for my blog.
Also, both are [Perl] based and I just don't write enough Perl these days.  Not
to mention the fact that I went and bought the domain and I just can't let it
go to waste.

[Contenticious]: http://memowe.github.io/contenticious/
[Mojolicious]: http://mojolicio.us
[Perl]: http://www.perl.org
[The Grinder]: http://grinder.sourceforge.net/
[Grinder Analyzer]: http://track.sourceforge.net/analyzer.html
[linux.conf.au]: http://linux.conf.au/
[The Perl Renaissance]: http://lanyrd.com/2013/linuxconfau/szzxt/
[meta::cpan]: https://metacpan.org/
[perl brew]: http://perlbrew.pl/
[cpanm]: http://cpanmin.us/
[Moose]: https://metacpan.org/module/Moose
[Dancer]: http://www.perldancer.org/
[Plack]: http://plackperl.org/
[Task::Kensho]: https://metacpan.org/module/Task::Kensho
[Dist::Zilla]: https://metacpan.org/module/Dist::Zilla
[Regexp::Debugger]: https://metacpan.org/module/Regexp::Debugger
[Plague Inc]: https://play.google.com/store/apps/details?id=com.miniclip.plagueinc
[DevAppsDirect]: https://play.google.com/store/apps/details?id=com.inappsquared.devappsdirect
[DayToDay]: https://itunes.apple.com/WebObjects/MZStore.woa/wa/viewSoftware?id=596623324&mt=8
[AOSP]: http://source.android.com/
