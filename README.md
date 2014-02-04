Selenium Server (Hub and Node) Services Scripts
===============================================

Introduction
------------

This module helps to build simple to set-up services for Selenium Grid(2).

Basically, it uses maven to fetch relevant files from internet and to
prepare a compressed archive holding a ready to be used on installed service
for a specific OS, thanks to [Java Service Wrapper](http://wrapper.tanukisoftware.com)

Thanks to [Java Weblog](http://javanetspeed.blogspot.com) for initial
[inspiration](http://javanetspeed.blogspot.com/2012/10/running-selenium-grid-as-service.html).

How it works
------------

This module will use maven to:

- fetch desired version of standalone Selenium Server JAR file
- fetch desired version of Java Service Wrapper
- build required packages to run a hub or grid node on Windows and Linux

So, basically, it should be only required a working Maven in order to use it.

Know Issues
-----------

- ***General***
    + maybe...
- **Windows**
    + maybe...
- **Linux**
    + maybe...