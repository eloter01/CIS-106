![banner](finalProjBanner.png)

## Table of Contents
- [Summary and Background](#summary-and-background)
- [System Specifications](#system-specifications)
- [Installing Samba](#installing-samba)
- [Samba Set Up](#samba-set-up)
- [Set Up User Accounts](#set-up-user-accounts)
- [Connect to Server in Linux client](#connect-to-server-in-linux-client)

- [Works Cited](#works-cited)

## Summary and Background
This guide will demonstrate the installation and configuration of a Samba server on Ubuntu for file sharing within the local network. Samba is open source and free software suite providing print and file service to SMB/CIFS clients over a number of different operating systems. This case will cover access to the file server for a Linux client over LAN.

## System Specifications
This installation and configuration of Samaba was completed on a virtual machine with the following specifications:

* OS Version: Ubuntu 20.04.2 LTS, 64-bit
* Memory: 1.9 Gib
* Processor: AMD Ryzen 5 4500u with radeon graphics x2
* Disk Capacity: 53.7 GB

## Installing Samba
To update package index and install the latest version of Samba, use the following commands:

`sudo apt update`
`sudo apt install samba`

The latest stable version of Samba is 4.14.4. To check the version installed, we run:

`smbd --version`

## Samba Set Up
This next section will cover the relevant commands and protocols to run for setting up the Samba file server.

1. Create a shared directory for Samba to use: 

![shared_folder](shared.png)

2. Add newly created directory to Samba configuration file. It can be opened with a text editor like Vim:

`sudo vim /etc/samba/smb.conf`

And add the following lines at the bottom and replace \<username> and \<sharedfile> with your local names:

    [sambashare]
        comment = Samba on Ubuntu
        path = <your shared directory path>
        read only = no
        browsable = yes

![sambaConfig](sambaConfig.png)

Comment describes the shared set up with Samba, path is the absolute path to your shared directory, read only grants permission to modify contents, and browsable allows the directory to be listed under "Network" in Ubuntu's default file manager.

Make sure to save before exiting!

3. Restart Samba and allow for Samba traffic under firewall rules:

`sudo service smbd restart`
`sudo ufw allow samba`

Here we are requesting restart of the service smbd, and to allow samba through the firewall.

## Set Up User Accounts

1. Set up a Samba access password for clients:

`sudo smbpasswd -a <username>`

Replace \<username> with a system account user running the server in order to save properly! You will be asked to create a password for a client to access the server.

2. Enable the client:

`sudo smbpasswd -e USER`

where USER is the name of the user account set up in the last step.

## Connect to Server in Linux client

1.  Check ip address of server by running ifconfig in Terminal:

`ifconfig`

![ipaddress](ipaddress.png)

Take note of the your ip address from above.

2. Open default file manager and enter server information from previous steps and configuration below:

![sambaConnect](sambaConnect.png)
![sambaConnect2](sambaConnect2.png)


## CONGRATULATIONS! You have set up and connected to your own Samba file server!

## Works Cited

1. “Install and Configure Samba.” Ubuntu, ubuntu.com/tutorials/install-and-configure-samba. 
2. Linuxize. “How to Install and Configure Samba on Ubuntu 18.04.” Linuxize, Linuxize, 27 Jan. 2019, linuxize.com/post/how-to-install-and-configure-samba-on-ubuntu-18-04/. 
3. Samba Documentation, www.samba.org/samba/docs/. 
4. Wallen, Jack. “How to Create a Samba Share on Ubuntu Server 20.04.” TechRepublic, TechRepublic, 17 Dec. 2020, www.techrepublic.com/article/how-to-create-a-samba-share-on-ubuntu-server-20-04/. 








