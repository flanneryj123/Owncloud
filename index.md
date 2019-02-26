#Quick Start Guide for ownCloud
This guide describes how to quickly install and configure your ownCloud server and how to connect to it from a client. This will help you to get familiar with ownCloud and let you verify that some basic user and connection settings are correct.

##About this Guide

###Audience
The intended audience for this guide are new users who want to complete a basic set up of the Appliance version of the ownCloud server. 

###Overview
To complete this quick start, you need to install the ownCloud server and connect to it from a mobile or desktop application. 

There are a number of dofferent options for installing the ownCloud server:

a. Tarball distributions: These are the most commonly used as they offer the most customisation options. This is best for production environments.
b. Docker image: These images are designed for experienced users who work in dockerized environments
c. Appliance: The appliance is the easiest way to install the server. You use it with Virtualization software such VirtualBox. It is    the best option for inexperienced users. This is the option that we will use in this guide
d. Linux distribution packages: Specific packages are available for popular distributions of Linux such a Red Hat Enterprise Linux. 
e. Hosted servers: A number of web service providers offer ownCloud installations as part of their web hosting offerings. 
 
For more information about each of these options, see [Download ownCloud](https://ownCloud.org/download/#ownCloud-server-tar-ball)

You can also download the desktop or mobile client from [the same link](https://ownCloud.org/download/#ownCloud-server-tar-ball)

This guide assumes that you will install the Appliance version of the ownCloud server and that you will connect to it with a desktop or mobile client. 

This quick start guide consists of the following tasks:

1. Install the ownCloud server 
2. Enable user connections
3. Add a user account
4. Connect to the server using a desktop or mobile client

##Installing
###System requirements
For the list of system requirements, see https://doc.ownCloud.com/server/admin_manual/installation/system_requirements.html

###User requirements
Ensure that the user who installs the server is an Administrator. 

###Downloading
Download the ownCloud Appliance image and the desktop or mobile client from {here](https://ownCloud.org/download/#ownCloud-server-tar-ball)

You also need to download either a desktop or mobile client from here. You will use this to test the connection to your server. 

##Installing and configuring the ownCloud Server

The following steps are a summary of the required steps for setting up the Appliance. The detailed steps are available [here] (https://doc.ownCloud.com/server/admin_manual/appliance/installation.html) 

Before you begin, ensure that you have downloaded the required virtualization tool. This example uses VirtualBox. 

To install the ownCloud server Appliance: 

1. Download the Appliance image from [here](https://ownCloud.org/download/#ownCloud-server-tar-ball) . Select the one that is appropriate for your virtualization software. 
2. After the download completes, click the file. 
3. Click Import Appliance and import the Univention-App-ownCloud-virtualbox.ova file. This is a large file so it may take some time to download. 
4. Import the file and accept the licence agreement. 


