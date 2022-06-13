
# Connecting EC2 Instance Public Server to EC2 Private Server 

## Introduction

This is a Whizlab challenge.



## Cloud Research

Here are the screenshot of the steps in the challenge:

![image](https://user-images.githubusercontent.com/99172259/173389398-3645d5e5-634d-4b33-ac6f-dbecc48c8bd7.png)


![image](https://user-images.githubusercontent.com/99172259/173389553-8923d616-a35f-4404-b6ba-d27e6588ba98.png)


After we create the VPC, subnet, route table, Internet Gateway, NAT Gateway and EC2 with public subnet and EC2 with private subnet. We have to perform ssh from the public ec2 server to the private ec2 server and run this commamd:

![image](https://user-images.githubusercontent.com/99172259/173389610-583c6c61-0074-4f93-a4d5-3113204301fc.png)

Actually, I managed to install the httpd but in the end I failed the task. I have no idea why it failed.

**Notes on ssh commands:**
- Before ssh to a private subnet instance, store the primary key file into the public server

nan0 filename.pem

- Then ssh with the pem

sudo ssh ec2user@hostip -i filename.pem


 
## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1535640011646697472)
