

# Network Fundamental (Ahmad Rosid Komarudin on Aguna Course) Day 4

## Cloud Research

**Subnetting Exercise**

Private IP

10.0.0.0 - 10.255.255.255 

172.16.0.0 - 172.31.255.255 

192.168.0.0 - 192.168.255.255

If there are 12 Pcs, so

Prefix : /28

it comes from 32 - 4

Total IP : 16 (2 to the power of 4)
Subnetmask : 256 - total IP so 256 - 16 = 240  > 255.255.255.240
IP Network   : 0    16    32    48  xxxxxx     > 192.168.1.0
IP Broadcast : 15   31    47    63  xxxxxx     > 192.168.1.15

So, IP range that we can use to configure
192.168.1.1 - 192.168.1.14
192.168.1.17 - 192.168.1.30     Block Subnet
192.168.1.33 - 192.168.1.46
xxxxxxxxxx

We can prove using CPT by inputing the IP address and subnet mask n ping it.

We cant use IP Network
![IP Network error](https://user-images.githubusercontent.com/99172259/154640440-7ebc9811-d5e6-4727-bac8-da4b972e7c8b.png)


We cant use IP broadcast
![IP Broadcast  error](https://user-images.githubusercontent.com/99172259/154640303-04805fea-d18d-446b-a217-8897b163f0dd.png)

Ping is successful since the IP range is used in both PC

![Ping success](https://user-images.githubusercontent.com/99172259/154640577-b8db54e1-45e3-4b05-8433-a0e33a6564ed.png)

**Block Subnet Concept**

Block Subnet is IP range that may be used in a network. So, those IP can interact each other. If the IP from two different block cannot interact. We can use the CPT to prove it.

![error block subnetting](https://user-images.githubusercontent.com/99172259/154640742-0b2a9f67-511e-4eb5-82b3-6a5449c399e2.png)

In conclusion, the IP configured in the same room should contain the ip number within the same subnet block. We have already found the subnet block before

192.168.1.1 - 192.168.1.14      Block subnet 1

192.168.1.17 - 192.168.1.30     Block Subnet 2

192.168.1.33 - 192.168.1.46     Block Subnet 3

## Social Proof

[Twitter](link)
