

# ENI & EC2 Hibernate (An SAA Course by Stephane Maarek)


## Cloud Research

### Elastic Network Interfaces (ENI)

Logical component in a VPC that represents a virtual network card

ENI can be created independently and attached on the fly (move them) on EC2 instances for failover

Bound to a specific availability zone (AZ)

### EC2 Hibernate

Hibernate EC2 instance so that when when it is started, it will boot faster since the OS is not stopped / restarted)

Condition

Supported Instance Families – C3, C4, C5, I3, M3, M4, R3, R4, T2, T3, …
• Instance RAM Size – must be less than 150 GB
• AMI – Amazon Linux 2, Linux AMI, Ubuntu, RHEL, CentOS & Windows… 
• Root Volume – must be EBS, encrypted, not instance store, and large
• Available for On-Demand, Reserved and Spot Instances
• An instance can NOT be hibernated more than 60 days



## Social Proof


[twitter](https://twitter.com/JoeSeven08/status/1539943114021908483)
