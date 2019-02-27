# Quick Start Guide for ownCloud

ownCloud is an open source file synching and sharing application. 

## About this Guide

This guide describes how to quickly install and configure your ownCloud server and connect to it from a mobile or desktop client. 

### Audience

The intended audience for this guide are new users who want to complete a trial set up of the Appliance version of the ownCloud server. Completing this guide will help you to become familiar with ownCloud. In this guide, we will install the Appliance image. This image includes prepackaged software like ownCloud X Server and Enterprise Apps, Apache 2, PHP, and MySQL to help you to get started quickly.

## Overview

### Deployment options

There are a number of deployment options:

+ Tarball distributions: These are the most commonly used as they offer the most customisation options. This is best for production environments.
+ Docker images: These images are designed for experienced users who work in dockerized environments.
+ Appliance images: These images are the simplest way to install the server. You use it with Virtualization software such VirtualBox. It is the best option for inexperienced users. This is the option that we will use in this guide.
+ Linux distribution packages: Specific packages are available for popular distributions of Linux such as Red Hat Enterprise Linux. 
+ Hosted servers: A number of web service providers offer ownCloud installations as part of their web hosting offerings. 
 
For more information about each of these options, see [Download ownCloud](https://ownCloud.org/download/#ownCloud-server-tar-ball).

You can also download the desktop or mobile client from  the same [link](https://ownCloud.org/download/#ownCloud-server-tar-ball).

### Assumptions

This guide assumes that you will install the Appliance image of the ownCloud server and that you will connect to it with a desktop  client. 

### Documentation and information
The documentation for ownCloud is [here](https://doc.owncloud.com/server/).

The documentation for the Appliance is [here](https://doc.owncloud.com/server/admin_manual/appliance/what-is-it.html).

For an overview of this guide with screenshots, you can also download the [White Paper for Appliance](https://oc.owncloud.com/rs/038-KRL-592/images/Whitepaper_User_Guide_Appliance_ENG.pdf) PDF document. 

## Installation

### Introduction

To ensure complete installation, complete the following steps:

1. Review the system requirements.
2. Install and configure the server.
3. Activate the licence.
4. Create ownCloud users.
5. Install the desktop or mobile client.


### System requirements

For the list of system requirements, see [System Requirements](https://doc.ownCloud.com/server/admin_manual/installation/system_requirements.html).

### Installing and configuring the server

The following steps are a summary of the required steps for setting up the Appliance. The detailed steps are documented [here](https://doc.ownCloud.com/server/admin_manual/appliance/installation.html) 

Ensure that you have downloaded the required virtualization tool. This example uses VirtualBox.  

To install and configure the server: 

1. Download the Appliance image from [here](https://ownCloud.org/download/#ownCloud-server-tar-ball). Select the one that is appropriate for your virtualization software. In this example, we are using VirtualBox.
2. After the download completes, click the file.
3. Click *Import Appliance* and import the "Univention-App-ownCloud-virtualbox.ova" file. This is a large file so it may take some time to download. 
4. Import the file and accept the licence agreement. 
5. Select the imported image and click *Start*. Allow time for the server to start. In most cases, 5 seconds is sufficient. 
6. The Configuration Wizard is displayed. Use it to review the localization settings, domain setup, account information and host settings. The password that you enter here is the root password for the virtaul machine that you are accessing. Note any passwords and the IP address of the server. 
7. To complete the configuration, click Finish. 

### Activating the licence

After you complete the installation and configuration, you need to activate your licence. The licence data is sent to the email address that you entered during configuration. Open a browser and enter the IP address of the server. Click *Upload licence file* and add the licence data from the email. 

### Creating ownCloud users

Next you need to create some ownCloud users to test the connection to the server:

1. After you activate the licence, you are redirected to the Portal. If you are not, enter the following https://\<ip address>/univention-management-console where \<ip_address> is the IP address of the server that you created.
2. Click on the *System and domain settings* tile. 
3. Log in with the Administrator user and password that you entered previously. 
4. To create users, click *Add:User* and create the users as required. It is recommended that you select the checkbox that requires users to reset their initial password for security reasons.

### Installing the desktop or mobile client

Finally, you need to download and install the desktop or mobile client and test the connection to the server. In this example, we will download the Desktop Cient. 

1. Download the Desktop Client from [here](https://ownCloud.org/download/#ownCloud-server-tar-ball).
2. To run the application, click the downloaded file. 
3. Enter the IP address of your ownCloud server in the *Server Address* field. 
4. Enter a user name and password. Use one of the ownCloud users that you created in the previous section.
5. To verify that the connection is working, you can create a new folder and place a file in it. 

You are now ready to begin using your ownCloud server. For more information, see the [User's Manual](https://doc.owncloud.com/server/user_manual/).
