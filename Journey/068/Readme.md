


# S3 Replication Demo & Pre-Designed URL

## Cloud Research

### S3 Replication Demo

You can have a broader knowledge regarding what S3 replication is and what the benefits are by reading this source from AWS https://docs.aws.amazon.com/AmazonS3/latest/userguide/replication.html

In conclusion S3 Replication is to replicate our object to the same region (SRR) or it can be directed to a different region (CRR). It can also be directed to other AWS account as well. 

Having practiced to create S3 replicated from US-east-1 to AP-southeast-3.I followed Adrian Cantril's instruction to create this demo. Here are the steps:

**Creating bucket as the source bucket**
- Creating S3 bucket in US-East-1


**Creating bucket as the destination bucket**
- Creating S3 bucket in AP-Southeast-3


**Setting the Replication**
- Go to the source bucket
- Click management
- Click create replication rule
- Enable bucket versioning
- Create a new IAM role
- Leave other as a default

**Creating a static web hosting in the source bucket**
- Upload the web file
- Host a static web hosting by configuring the propeties and update the bucket policy



### Pre-signed URL

- Generally S3 bucket is private
- The pre-designed URL is to enable someone or device to access your S3 within a time limit
- Use cases (Stephane Maarek - SAA Course on Udemy):
• Allow only logged-in users to download a premium video on your S3 bucket
• Allow an ever changing list of users to download files by generating URLs dynamically
• Allow temporarily a user to upload a file to a precise location in our buckeT
- For more info : https://docs.aws.amazon.com/AmazonS3/latest/userguide/ShareObjectPreSignedURL.html


## ☁️ Cloud Outcome

### S3 Replication Demo Result

**Source bucket static web hosting**

![image](https://user-images.githubusercontent.com/99172259/173714220-0172a38c-00b7-4113-b20d-4b1da31e39a7.png)


**Destination bucket static web hosting**

![image](https://user-images.githubusercontent.com/99172259/173714831-6b05b320-d96b-4170-96cf-477b08f611e4.png)


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1536870867929804801)
