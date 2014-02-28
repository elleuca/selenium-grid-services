Install Selenium Grid Service on Linux
======================================

Requisites
----------

- working `java` command (to run the service/daemon)
- a static IP for nodes and hub hosts
- admin privileges (to install as system service/daemon)

Overview
--------

Steps are

1. Extract the package (for instance under `/opt` if you want to run a system service)
1. Configure IP
1. Execute the installer
1. Start the service (or reboot the machine)

Extract the package
-------------------

Change to machine/directory you like to use to hold Selenium Grid Server installation and extract the relevant package.
For instance, to install the Selenium Hub Service, on target system do as following:

- change to directory: 
    `cd /opt/`
- extract the file:
    `sudo tar xvf /path/to/file/selenium-node-service-0.0.3-linux-x86-64.tar.bz2`

Configure IP
----------------------------

Edit `conf/hub.json` or `conf/node.json` file and replace both @FILL_ME_WITH_IP@ with the IP of the hub you'll connect the node and the IP of the node itself.

This is the only needed configuration step in deployment phase. Please note you could need a "static" address (DHCP is fine is you always have the same IP) and you should run the hub/node service wrapper *after* the IP is available.

Execute the installer
---------------------

If you like to run Selenium Grid Service as a system service/deamon, please run `sudo ./bin/nodeservice install` or `sudo ./bin/hubservice install` on command line from extracted package directory.

More options are available, add `--help` and see.

If you plan to manually run the service when needed, you can skip to next step.

Start the service
-----------------

The first time after installation you have to manually launch the service.

You can use any method provided by your Linux distribution, for example `sudo service ??????? start`

