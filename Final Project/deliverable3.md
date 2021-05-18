

![banner](finalProjBanner.png)

<!-- TOC -->autoautoauto<!-- /TOC -->

## Summary and Background
This article will demonstrate the installation and configuration of a Samba server on Ubuntu for file sharing via the local network. Samba is open source and free software suite providing print and file service to SMB/CIFS clients over a number of different operating systems. This case will cover access to the file server for Windows clients.

For operating a file server, the two relevant programs in the suite are:
* smbd: the server daemon that provides file sharing and printing services to Windows clients.
* nmbd: NetBIOS name service and browsing daemon.

## System Requirements
The following is required for this tutorial:
* Ubuntu 16.04 LTS
* Available Local Area Network (LAN) over which to share files

## Installing Samba
To update package index and install the latest version of Samba, use the following commands:
`sudo apt update`
`sudo apt install samba`

The latest stable version of Samba is 4.14.4. To check the version installed, run:
`smbd --version`

To verify the Samba services are running, use:
`systemctl status smbd nmbd`

If they are not, run the following commands to get started:
`sudo systemctl start smbd nmbd`


## Samba Set Up
This next section will cover the relevant commands and protocols to run for setting up the Samba file server.




