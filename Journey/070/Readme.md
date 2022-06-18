
# VPC Sizing & Structure

## Cloud Research

### CIDR

CIDR is the short for Classless Inter-Domain Routing, an IP addressing scheme that replaces the older system based on classes A, B, and C. A single IP address can be used to designate many unique IP addresses with CIDR. A CIDR IP address looks like a normal IP address except that it ends with a slash followed by a number, called the IP network prefix. CIDR addresses reduce the size of routing tables and make more IP addresses available within organizations.

**CIDR in IPV4**

- CIDR consists of two components namely base ip and subnet mask
- Base IP (represent an ip contained in the range) example : 10.0.0.0
- Subnet mask IP (defines how many bits can chage in the IP) example : /32 or 255.255.255.255, /24 0r 255.255.255.0, /16 or 255.255.0.0, /8 or 255.0.0.0. For the detail can be seen in the table below

![image](https://user-images.githubusercontent.com/99172259/174418069-69d77cd8-cfe9-4b5d-ac82-3bf0561abcb8.png)

CIDR to IPv4 Conversion tools: 

https://www.ipaddressguide.com/cidr



### VPC

on-demand configurable pool of shared resources allocated within a public cloud environment, providing a certain level of isolation between the different organizations (denoted as users hereafter) using the resources. The isolation between one VPC user and all other users of the same cloud (other VPC users as well as other public cloud users) is achieved normally through allocation of a private IP subnet and a virtual communication construct (such as a VLAN or a set of encrypted communication channels) per user. In a VPC, the previously described mechanism, providing isolation within the cloud, is accompanied with a VPN function (again, allocated per VPC user) that secures, by means of authentication and encryption, the remote access of the organization to its VPC resources. With the introduction of the described isolation levels, an organization using this service is in effect working on a 'virtually private' cloud (that is, as if the cloud infrastructure is not shared with other users), and hence the name VPC. (https://en.wikipedia.org/wiki/Virtual_private_cloud)

**Amazon Virtual Private Cloud (Amazon VPC)** enables you to launch AWS resources into a virtual network that you've defined. This virtual network closely resembles a traditional network that you'd operate in your own data center, with the benefits of using the scalable infrastructure of AWS.

**VPC Consideration**

- What size should the VPC be
- Because VPC is private, only the Private IPV4 ranges are allowed
  10.0.0.0/8 (10.0.0.0 - 10.255.255.255)
  
  172.16.0.0/12 (172.16.255.255 - 172.31.255.255)
  
  192.168.0.0/16 (192.168.0.0 - 192.168.255.255)
 
- Think of IP ranges to avoid so there is no overlapping IP address
  
  For example, we want to create a new vpc for the branch office but our office has had these IP addresses attached to their network:
  
  10.0.0.0/16 (AWS) (10.0.0.0 - 10.0.255.255)
  
  192.168.15.0/24 (Head Office) (192.168.15.0-192.168.15.255)

  So, we have to create a network that has different private IP range than those IP. For instance, 192.168.16.0/24

**More VPC Consideration**

- We can have multiple VPCs in an AWS region (max. 5 per region)
- Max.CIDR per VPC is 5, for each CIDR
  
  min. size is /28
  
  max size is /16

**VPC Structure**

- In AWS, one region can consist of 3 AZ for minimum
- We will have 4 tier design which are web,application, data base, spare



## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1537473945288704000)
