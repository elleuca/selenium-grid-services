Selenium Server (Hub and Node) Services Builder
===============================================

Introduction
------------

This module helps to build simple to set-up services for Selenium Grid(2).

Basically, it uses Maven to

 *  fetch desired version of standalone [Selenium Server](http://docs.seleniumhq.org/download/) JAR file
 *  fetch desired version of [Java Service Wrapper](http://wrapper.tanukisoftware.com)
 *  build packages to install/run a hub or grid node on Windows and Linux

Thanks to [Java Weblog](http://javanetspeed.blogspot.com) for initial
[inspiration](http://javanetspeed.blogspot.com/2012/10/running-selenium-grid-as-service.html).

Getting Started
---------------

* clone this repository (`master` branch holds stable release)
* run `mvn package`
* pick up packages from `hub/target` and `node/target` subdirectories
* follow instructions in `README` and `INSTALL` files to run or install services

By now node and hub packages for Linux (x86-64) and Windows (x86-32) are provided.

Package Usage
-------------

**Important** in order to have a working grid, you have to *configure* each node service providing IP addresses
for hub host and for node host itself.

Steps to set up a hub/node host are:

* extract package
* configure it if it's a node host (see `conf/node.json`)
* manually run or install as a service (see `bin/`

Detailed info are available in `README` and `INSTALL files.

Know Issues
-----------

Please see [Issue Tracker](https://bitbucket.org/elleuca/selenium-grid-services/issues?status=new&status=open) for
updated info about existing issues.

Of course, feel free to to report any issue you found, we'll try to fix it ASAP, and to fork this module and improve it
(yes, a github copy is planned)

Licence
-------

Hmmmm... Dunno... it's just a build system, I've to check which one (OpenSource, of course) will fit better ;-)