
# Network Fundamental (Ahmad Rosid Komarudin on Aguna Course) & Simulating How to Create Instance using Lightsail

## Introduction

I continue the network fundamental course and my superior taught me to create instance using lightsail. The lightsail session is a sharing session from my superior so that I can realize that cloud computing is an instant process!  

## Cloud Research

**AGUNA COURSE**
- Determining the most effective prefix

/24 means 256 for the total IP

 32 -24     8
2       >  2   = 256

Why 32? because ip address in total are 32. It is based in binnary way. So, if there are 12 cpu in a room the most appropriate prefix is /28. it is derived from 32 - 28 = 4 so 2.2.2.2 is 16.

- Subnetting 1 - Total IP & Subnetmask

Here I learnt how to count the total ip and how to search for subnetmask number. 

Total IP can be counted this way. For example there are 100 pc in a room and we need to decide the total IP. We can count
 32-25   7
2      =2   = 128
Meanwhile, ways to count subnetmask is like this way
256 - total IP
256 - 128 = 128

So, when we need to input subnetmask in the IP configuration, we can put 255.255.255.128

- IP Network

The first IP in the network and it must be 0

- IP broadcast 

The last IP in the network. It depends on the total IP. Lets say there are 128 IPs then the last number is 127. And we also need to decide how many block IP we can use. How to count it? We use the previous case about 100 pcs in a room.
First block
0 (IP network) - 127 (IP broadcast)
Second block
128 (IP network) - 255 (IP broadcast)

- IP range 

IP that can be used in configuration. IP network and IP broadcast cant be used.  So, if we have counted the total IP and determine the block, the IP available are 1-126 for the first block 129- 254 for the second block. 

**Sharing Session about Lightsail (Creating instance instantly using AWS)**

Here we would like to create instance. We can choose where the location of the server is, the OS and also the apps. Just click create instance, then it is done. It is super faster than ever!

## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1494332530845417473)
