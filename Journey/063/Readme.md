

# Deploying FreeNAS on Virtualbox

## Introduction

What is network-attached storage (NAS)?
Network-attached storage (NAS) is dedicated file storage that enables multiple users and heterogeneous client devices to retrieve data from centralized disk capacity. Users on a local area network (LAN) access the shared storage via a standard Ethernet connection.

source : https://www.techtarget.com/searchstorage/definition/network-attached-storage

## Cloud Research
The steps I did, based on YT video. Source : https://www.youtube.com/watch?v=1HtdjoCaMtk


**Creating a machine on VirtualBox**

- Select BSD as the OS, use 64 bit version, previously I used 32 bit and it failed
- The suggested memory size is 6 Gb but I chose 1 Gb
- For the storage I set 16 Gb
- Kindly set up the network to Bridged adapter so that the vm can connect using your wifi laptop
- Also create additional hard disk 

here is the result

<img src= https://user-images.githubusercontent.com/99172259/172029687-f3ad3eac-6899-4f64-a109-de56f66cdc7a.png width="800" height="550" />

**Installing FreeNAS in the Machine**
- Previously you can download the FreeNAS on this link https://downloads.digitaltrends.com/freenas/windows
- Start the machine you just crated
- Insert the disk. 
<img src= https://user-images.githubusercontent.com/99172259/172029803-71dad2d0-27ee-438e-abf0-5cf1abc93ffc.png width="300" height="250" />

- Reset the machine
- Wait until the installation ends. Before it ends, you will need to configure the password
- Type in the http site that is provided at the end of the installation process
- When login, the username is root. For the password, it was the same as it was set at the configuration step

Here is the result:

![Screenshot (517)](https://user-images.githubusercontent.com/99172259/172029865-3fb5a3c7-1663-4ba8-9e9c-c0542d4bd04f.png)


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1533243761186471936)
