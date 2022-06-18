

# Subnet & Creating VPC


## Cloud Research

### VPC-Subnet (AWS-SAA by Course Stepahane Maarek)

• AWS reserves 5 IP addresses (first 4 & last 1) in each subnet
• These 5 IP addresses are not available for use and can’t be assigned to an EC2 instance
• Example: if CIDR block 10.0.0.0/24, then reserved IP addresses are:
• 10.0.0.0 – Network Address
• 10.0.0.1 – reserved by AWS for the VPC router
• 10.0.0.2 – reserved by AWS for mapping to Amazon-provided DNS
• 10.0.0.3 – reserved by AWS for future use
• 10.0.0.255 – Network Broadcast Address. AWS does not support broadcast in a VPC, therefore the address is reserved

### Creating VPC (AWSS SAA Course by Adrian Cantrill)

Here I created vpc in US-East-1 region with 12 subnets:

![image](https://user-images.githubusercontent.com/99172259/174430510-1d8cf910-9980-4710-b45c-32456419742f.png)

### VPC - Route Table

- Every VPC has a vpc router
- Route traffic between subnets
- It can be attached to one main route tables and associated with many subnets

**Creating public and private route tables**

Public route table example

1. Click on route table

<img src=https://user-images.githubusercontent.com/99172259/174432250-78663c0e-4092-4c08-890e-f9f4c022650c.png width="500" height="500" />

2. Fill in the name and click create route table

<img src=https://user-images.githubusercontent.com/99172259/174432387-a24b9622-cc44-4fd5-83c1-f7e80f830c5c.png width="500" height="200" />


3. Associate the subnet

<img src=https://user-images.githubusercontent.com/99172259/174432509-d2c2a9cb-80d6-4e68-bd3c-7e6d376d720e.png width="500" height="200" />

4. Choose the subnet and save

<img src=https://user-images.githubusercontent.com/99172259/174432577-85f4c12a-b801-4117-a4b6-097dd91e2e04.png width="500" height="200" />

5. Add internet gateways and update the route table
6. Edit subnet settings

<img src=https://user-images.githubusercontent.com/99172259/174433124-730365d4-9df6-41dc-9650-27f363e3b010.png width="500" height="200" />

7. Thick enable auto assign public ip

<img src=https://user-images.githubusercontent.com/99172259/174433175-cb2ed6d5-86e1-43f4-8a1e-e7829a69b913.png width="500" height="500" />





### Internet Gateways

- It is needed to make the public subnet in a vpc connect to the internet
- Creating internet gateways:

1. Choose internet gateways

<img src=https://user-images.githubusercontent.com/99172259/174431783-abbfaf25-f521-4a34-80ee-026ee3d21e11.png width="500" height="200" />

2. Fill in the name and click create internet gateways


<img src=https://user-images.githubusercontent.com/99172259/174431988-8eb3b251-79ff-4e2c-b1c1-9e55782135a5.png width="500" height="500" />

3. Attach to a vpc

<img src=https://user-images.githubusercontent.com/99172259/174432114-11949bcf-6d1c-48c8-b44b-a291c0168ef7.png width="500" height="200" />

4. Edit the vpc route table

<img src=https://user-images.githubusercontent.com/99172259/174432936-ddb59b15-e800-4fc4-b342-8ee9709ec5b1.png width="500" height="200" />

4. Configure the ip and set the target as internet gateway

<img src=https://user-images.githubusercontent.com/99172259/174432829-ed2ea663-f5aa-4b2d-80b6-64c99703ebd7.png width="500" height="200" />

5. 


### Bastion Host/Jumpbox

An instance in a public subnet

## Social Proof

[Twitter](link)
