

# DNS Record Type, Elastic IP and EC2 Placement Group 


## Cloud Research

**DNS records types**

Commonly used record types

A (Host address)
AAAA (IPv6 host address)
ALIAS (Auto resolved alias)
CNAME (Canonical name for an alias)
MX (Mail eXchange)
NS (Name Server)
PTR (Pointer)
SOA (Start Of Authority)
SRV (location of service)
TXT (Descriptive text)

Additional source:

https://www.jetorbit.com/panduan/mengenal-dan-mengetahui-jenis-jenis-dns-record

https://simpledns.plus/help/dns-record-types



**Elastic IP**

When we create EC2 instances, it will automatically give us public ip. However, the public ip will change once we stop the instance and start it again. So, to overcome this, we have to associate an elastic IP to our EC2 instance.

Applying Elastic IP on EC2 Instances

It has easy steps. Just click on elastic IP and allocate elastic ip. After creating it, associate with the instance. 

![image](https://user-images.githubusercontent.com/99172259/170452778-6a8ea2ad-9b67-4c9a-b9ba-e8f752f1d8de.png)

![image](https://user-images.githubusercontent.com/99172259/170452902-1e9be391-86e1-4095-93e8-f90387c43b50.png)



**EC2 Placement Groups**

When we have more than one instance, we can apply a strategy that suits our goal. On the EC2 menu, we can create placement groups and each placement group offer different benefits. 


Cluster (Performance)

Spread (Resilience)

Partition (Topology Awareness)


![image](https://user-images.githubusercontent.com/99172259/170453018-d72646b9-71cc-457f-84c2-47de5bed1d52.png)

![image](https://user-images.githubusercontent.com/99172259/170453077-49bb8154-970a-43fa-aee8-35f3dfe09e1f.png)


## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1529746841382047744)
