<img src=https://user-images.githubusercontent.com/99172259/174464046-ac5da56c-93bd-411a-aeda-d25d6c43ec0a.png width="1000" height="300" />

# NAT Instance vs NAT Gateway & NACL vs Security Group

## NAT Instance

### Cloud Research
 
**Definition**

NAT instance is used to connect the private instance into the public internet. NAT instance can be created based on NAT AMI. We can find NAT AMI in the AMI marketplace. 

**How to create it**
1. Launch EC2 instance
2. Find NAT AMI from the marketplace

<img src=https://user-images.githubusercontent.com/99172259/174464215-527ca1c2-0544-4484-9575-30fc238f7100.png width="600" height="200" />

3. Make sure that NAT instance is launched in the same vpc as the private instance and choose the public subnet.
5. Set the security group to allow http and https from the vpc

<img src=https://user-images.githubusercontent.com/99172259/174464417-5c0ac056-1337-49e8-8687-d9adcab8fd21.png width="600" height="200" />

6. Stop the source/destination check

a.

![image](https://user-images.githubusercontent.com/99172259/174464521-4119403e-bd29-434a-92b7-7a7831278c1f.png)


b. 

<img src=https://user-images.githubusercontent.com/99172259/174464546-d31b2043-2eba-4dea-a02a-a55effe2fdda.png width="700" height="300" />

7. Update the private route table

<img src=https://user-images.githubusercontent.com/99172259/174464622-2b8fd5fe-c2d6-40af-aa9b-7be5f7adf761.png width="700" height="300" />

8. Modify the security group of the NAT instance by adding all icmp rule in the inbound rule from the vpc

![image](https://user-images.githubusercontent.com/99172259/174464726-fff093d8-108c-4af0-8603-233ab2876e37.png) 

10. To prove it, connect to the private instance throught the bastion host. Ping google.com from the private instance.

<img src=https://user-images.githubusercontent.com/99172259/174464785-b2c0ac52-e220-48f8-997b-f489e3e195da.png width="700" height="300" />

## NAT Gateway

In case you do not need the NAT instance, you can set the NAT gateway for the private instance so that it can connect to the internet.

**How to configure it**

1. Create NAT Gateway and attach it to the public subnet

<img src=https://user-images.githubusercontent.com/99172259/174464905-4367e6cc-03d2-45b5-93ff-5ee6456432d6.png width="700" height="300" />

2. Update the route table

<img src=https://user-images.githubusercontent.com/99172259/174464932-3e9ce41b-7315-4bb3-88ca-91e2a50eb1e2.png width="700" height="300" />

3. To prove it, you can ping google.com from the private instance. You can ssh it through the bastion host.


<img src=https://user-images.githubusercontent.com/99172259/174465098-b80b3967-f78f-46bc-95d0-138cd84b8d40.png width="700" height="300" />


**Comparison between NAT gateways & NAT instances**

https://docs.aws.amazon.com/vpc/latest/userguide/vpc-nat-comparison.html


## Stateful vs Stateless Firewall


### Prerequisite

It is related to stateful and stateless firewall.

### Cloud Research


Stateful firewall means that when it is allowed for an ip to access (outbound) a destination ip the ip will be eligle to receive access (inbound) from the destination ip. While stateless is not automatically set the inbound and outbound rule. It needs to be set the inbound and outbond rule explicitly.


### NACL vs Security Group

**NACL**

A network access control list (ACL) is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. You might set up network ACLs with rules similar to your security groups in order to add an additional layer of security to your VPC.

It is stateless firewall.

For more detail :
https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html

**Security Group**

The rules of a security group control the inbound traffic that's allowed to reach the instances that are associated with the security group. The rules also control the outbound traffic that's allowed to leave them.

**Differences of SG & NACL based on Stephane Maarek**

![image](https://user-images.githubusercontent.com/99172259/174463688-614da2e1-6398-4f3a-89ba-af32468a1dd2.png)


**Conclusion Based on Hands-on**

- created a web server on a public subnet. Started the httpd and run this command
![image](https://user-images.githubusercontent.com/99172259/174465816-9a18a4ac-cf44-42f4-8b3d-d3e0df79fafc.png)
- Enable http in SG. Then it can be accessed from anywher

![image](https://user-images.githubusercontent.com/99172259/174465869-cc1102e4-03d2-42ed-a6e8-454d3f1f2ee9.png)

- modified the NACL inbound rule number. If the allow rule has lower number than deny rule, the allow rule is more prioritied and vice versa.

Setting

![image](https://user-images.githubusercontent.com/99172259/174465899-315cec04-be8f-4f1f-b111-9817be6a9c6d.png)

Result

![image](https://user-images.githubusercontent.com/99172259/174465909-5ef186b0-72c4-4e65-a888-44d5159a0db7.png)



- If the inbound rule on NACL is allow and the outbound rule on NACL is deny then it will not be accesible


- If the outbound SG for allowing http to anywhere is deleted and the inbound still allow http traffic from anywher, the outbound rule still works since SG is stateless.


## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1538375171123609600)
