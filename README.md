Class2Go 
-------------

Class2Go is the project codename for Stanford's internal platform
for hosting on-line courses.  We began building Class2Go in June
2012.  A team of eight has worked through the summer.  It will
launch in Fall 2012 for a handful of Stanford classes.

(TODO: list of classes, links here)

Class2Go is intended to be a platform for research.  Professors will
have direct access to the data for their classes to learn how their students
learn.  We will facilitate experiments to help teachers and
researchers learn how people learn.  This could be just simple A/B/N
testing, or even bespoke code to try out interesting new features.

If you are interested in discussing with us, the team can be reached 
at [class2go@cs.stanford.edu] [mail].

  [mail]: mailto:class2go@cs.stanford.edu

Philosophy and Key Features
-------------------------

Here is what is important to us.

* *Open*. The platform is open source to make it easier for users
    (faulty members) to give us feedback on what we are doing.
    Eventually we would love to have others use the platform, or
    to collaborate with similar efforts in other places.

* *Portable*. We believe strongly that the valuable course content
    shouldn't be tied to any one platform. Documents are already
    portable; the videos are outside our system (in YouTube) and
    the assets themselves can be repurposed as they see fit.  And
    our exercises and problem sets, instead of being trapped in a
    proprietary database, are in the Khan Academy format, so they
    can be used elsewhere.

* *Interoperable*. We don't want to build or maintain more than we
    have to.  See the section below for a list of all the shoulders
    we are standing on.

To bring this to life then we've built a few key features:

* *Content Management*. We have build a simple content management
    system where course information (videos, static pages, problem
    sets) can be created, reviewed, and then published.  One important
    ability is an automatic live date, so a professor (or, most
    likely, a TA) doesn't have to click a button at midnight to
    publish a problem set.

* *Video and Problem Set Management*. Professors (and TA's) can
    upload assets to S3; videos are then uploaded to to YouTube.
    We have a simple video player, navigable

* *Frame Extraction*.  We have a tool for extracting frames from
    a video (using ```ffmpeg```) differencing them to find key
    frames, and then using as an index to the video.  We call it
    the Kelvinator because it was written by Kelvin.

* *Exercises*.  We support two kinds of exercises: formative (for
    learning) and summative (for assessment, like quizzes and tests).



Leveraging Others
-------------------------

Thanks to all the projects we are relying on to make this work.  Some
commercial, some open source.  But a ton of good stuff.

* [YouTube] [yt] for videos
* [Piazza] [pz] for forums
* [MySQL] [mysql] is our database
* The massive [Python] [p] [Django] [dj] ecosystem: eg. South, Registration
* [Amazon] [a] AWS suite for hosting (EC2, S3, Route53, IAM)
* Chef from [Opscode] [oc] for configuration management
* [Github] [gh] for source code management and issues

  [yt]:    http://www.youtube.com/
  [khan]:  http://www.khanacademy.org/
  [pz]:    http://www.mysql.org/
  [mysql]: http://www.mysql.org/
  [p]:     http://www.python.org/
  [dj]:    http://www.djangoproject.com/
  [a]:     http://aws.amazon.com/
  [oc]:    http://www.opscode.org/
  [gh]:    http://www.github.com/


License
-------------------------

TODO: license terms

