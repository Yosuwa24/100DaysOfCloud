

# MFA Activation, S3 Storage Classes, S3 Replication



## Cloud Research

### MFA Activation

It is a simple step to double secure your account. To setup, you can just go to IAM and type MFA below the dashboard and choose for which account MFA is assigned. 

MFA Virtual has several application options that can be based on Android or iOS phone.

![image](https://user-images.githubusercontent.com/99172259/173474305-a7a4a6f7-0d7b-4ff6-bffa-dfbb3ca686a3.png)

After you choose, enter 2 MFA key shown on your phone.

### Storage Classes

- Amazon S3 Standard - General Purpose

S3 Standard offers high durability, availability, and performance object storage for frequently accessed data. Because it delivers low latency and high throughput, S3 Standard is appropriate for a wide variety of use cases, including cloud applications, dynamic websites, content distribution, mobile and gaming applications, and big data analytics.

Use cases : Big Data analytics, mobile & gaming applications, content distribution

- Amazon S3 Standard-Infrequent Access (IA)

S3 Standard-IA is for data that is accessed less frequently, but requires rapid access when needed. S3 Standard-IA offers the high durability, high throughput, and low latency of S3 Standard, with a low per GB storage price and per GB retrieval charge. 

Use cases : Disaster Recovery, backups

- Amazon S3 One Zone-Infrequent Access

S3 One Zone-IA is for data that is accessed less frequently, but requires rapid access when needed. Unlike other S3 Storage Classes which store data in a minimum of three Availability Zones (AZs), S3 One Zone-IA stores data in a single AZ and costs 20% less than S3 Standard-IA.
Use cases : Storing secondary backup copies of on-premises data, or data you can recreate

- Amazon S3 Glacier Instant Retrieval

Amazon S3 Glacier Instant Retrieval is an archive storage class that delivers the lowest-cost storage for long-lived data that is rarely accessed and requires retrieval in milliseconds. 

- Amazon S3 Glacier Flexible Retrieval

S3 Glacier Flexible Retrieval delivers low-cost storage, up to 10% lower cost (than S3 Glacier Instant Retrieval), for archive data that is accessed 1—2 times per year and is retrieved asynchronously. 

- Amazon S3 Glacier Deep Archive

S3 Glacier Deep Archive is Amazon S3’s lowest-cost storage class and supports long-term retention and digital preservation for data that may be accessed once or twice in a year. 

- Amazon S3 Intelligent Tiering

Amazon S3 Intelligent-Tiering (S3 Intelligent-Tiering) is the first cloud storage that automatically reduces your storage costs on a granular object level by automatically moving data to the most cost-effective access tier based on access frequency, without performance impact, retrieval fees, or operational overhead. S3 Intelligent-Tiering delivers milliseconds latency and high throughput performance for frequently, infrequently, and rarely accessed data in the Frequent, Infrequent, and Archive Instant Access tiers. You can use S3 Intelligent-Tiering as the default storage class for virtually any workload, especially data lakes, data analytics, new applications, and user-generated content.


### S3 Replication

![image](https://user-images.githubusercontent.com/99172259/173475242-0373fdce-768f-40f5-afdd-719be822b10b.png)




https://aws.amazon.com/s3/features/replication/



## Social Proof



[Twitter](https://twitter.com/JoeSeven08/status/1536386424097738752)
