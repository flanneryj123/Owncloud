# Quick Start Guide for ownCloud

This guide describes how to quickly install and configure your ownCloud server and how to connect to it from a client. This will help you to get familiar with ownCloud and let you verify that some basic user and connection settings are correct.

## About this Guide

### Audience

The intended audience for this guide are new users who want to complete a basic set up of the Appliance version of the ownCloud server. 

### Overview

To complete this quick start, you need to install the ownCloud Appliance and connect to it from a mobile or desktop application. 

### Deployment options

There are a number of deployment options, including the Appliance image, that can be used to instal the ownCloud server:

*Tarball distributions: These are the most commonly used as they offer the most customisation options. This is best for production environments.
*Docker image: These images are designed for experienced users who work in dockerized environments
*Appliance image: The Appliance image is the easiest way to install the server. You use it with Virtualization software such VirtualBox. It is the best option for inexperienced users. This is the option that we will use in this guide
*Linux distribution packages: Specific packages are available for popular distributions of Linux such a Red Hat Enterprise Linux. 
"Hosted servers: A number of web service providers offer ownCloud installations as part of their web hosting offerings. 
 
For more information about each of these options, see [Download ownCloud](https://ownCloud.org/download/#ownCloud-server-tar-ball)

You can also download the desktop or mobile client from [the same link](https://ownCloud.org/download/#ownCloud-server-tar-ball)

### Assumptions

This guide assumes that you will install the Appliance image of the ownCloud server and that you will connect to it with a desktop or mobile client. 

### Documentation
The documentation for ownCloud is [here] ()

## Installation

### Introduction

This quick start guide consists of the following tasks:

1. Installing and configuring the ownCloud Appliance image
2. Enable user connections
3. Add a user account
4. Connect to the server using a desktop or mobile client


### System requirements

For the list of system requirements, see [System requirements](https://doc.ownCloud.com/server/admin_manual/installation/system_requirements.html) 

### User requirements

Ensure that the user who installs the server is an Administrator. 

### Downloading

Download the ownCloud Appliance image and the desktop or mobile client from {here](https://ownCloud.org/download/#ownCloud-server-tar-ball)
 
Ensure that you have downloaded the required virtualization tool. This example uses VirtualBox.  

### Installing and configuring the Appliance image

The following steps are a summary of the required steps for setting up the Appliance. The detailed steps are documented [here](https://doc.ownCloud.com/server/admin_manual/appliance/installation.html) 

To install and configure the ownCloud Appliance server: 

1. Download the Appliance image from [here](https://ownCloud.org/download/#ownCloud-server-tar-ball). Select the one that is appropriate for your virtualization software. 
2. After the download completes, click the file. 
3. Click Import Appliance and import the Univention-App-ownCloud-virtualbox.ova file. This is a large file so it may take some time to download. 
4. Import the file and accept the licence agreement. 
5. Select the imported image and click Start. Allow time for the server to start. In most cases, 5 seconds is sufficient. 
6. The Configuration Wizard is displayed. Use it to review the localization settings, domain setup, account information and host settings. Note any paswords and the IP address of the server. 
7. To complete the configuration, click Finish. 

### Activating the licence

After you complete the installation and configuration, you need to activate your licence. To do so, open a browser and enter the IP address of the server that you created in the previous step.

### Creating users

Next you need to create some users to test the connection to the server

1. After you activate the licence, you are redirected to the Portal. If you are not, enter the following https://<ip address>/univention-management-console where <ip_address> is the IP address of the server that you created.
2. Click on the System and domain settings tile. 
3. Log in with the Administrator user and password that you created previously. 
4. To create users, click Add:User and create the users as required. It is recommended that you select the checkbox that requires users to reset their initial password.

### Testing the desktop or mobile client

Finally, you need to download and install the desktop or mobile client and test the connection to the server. In this guide, we will download the Desktop Cient. 
1. Download the Desktop Client from {here](https://ownCloud.org/download/#ownCloud-server-tar-ball)
2. To run the application, click the downloaded file. 
3. Enter the IP address of your ownCloud server in the Server Address field. 
4. Enter a user name and password. 
5. To verify that the connection is working, you can create a new folder and place a file in it. 
