# Network Fundamental (Ahmad Rosid Komarudin on Aguna Course) & AWS Certified Cloud Practitioner Course (Stephane Maarek on Udemy): Day 2

## Introduction
I try to simulate how computer network works and try to cope with the AWS course also since already have a root AWS account. However I will focus on the network fundamental first. Here I just wanted to review what cloud computing is.

## Cloud Research
**AWS CCP**
- Traditional IT Overview
  
  Here is discussed about how the server was built. Server is composed of CPU,Memory,storage, database and network. Traditionally, each website had their own servers. Like google, it was built in their own garage. When their business grew, they moved to a bigger office so that they can have as many servers as possible. With the help of cloud they do not need to build their own servers. 
  
- What is cloud computing

  The key word is on demand. People can create how many servers as they need and pay as they go. They can create instantly. So, cloud computing is more efficient rather than the traditional server (private cloud)

Aguna Course
- Download & Install Cisco Packet Tracer

  Cisco pakcet tracer is a software to simulate computer netwrok. You can download it by sign up to netacad.com

- Doing simulation with CPT to make the simplest computer network

![Screenshot (480)](https://user-images.githubusercontent.com/99172259/154237381-666cdb9c-cd54-45ac-9c8c-5223d4fca19f.png)

Real simple. You just need to pick pictures. It illustrates the computer linked by LAN cable then I ping it and it works!

- Introduction to IP Address & Subnetting

Briefly, IP address is the name of a computer. It contain numbers and use this format : x.x.x.x . The numbers we can use are from 0 until 255. However there specific numbers for public IP and private IP. 
Format for IP Address:  x.x.x.x
  Number : 0-255
  examples : 192.168.1.1/24
correct ip address using prefix (/)

Subnetting is used to determine the most effective prefix that can be used

example: we have 6 computer in a classroom
which prefix is the best?
/24 means 256 ip
the most appropriate prefix is /29 since /29 consists of 8 ips.

- Public & Private IP

Public IP  is IP can be accessed on the internet like Youtube, facebook, google etc.


Private IP is IP in a local network. Example, there are 6 computers in an office in which each computer has their own IP private and they connected with each other. So, the IP can be accessed only from inside the office.
Range Private IP: 
10.0.0.0 - 10.255.255.255
172.16.0.0 - 172.31.255.255
192.168.0.0 - 192.168.255.255

outside the range of private ip is public ip, for example 13.1.1.1



## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
