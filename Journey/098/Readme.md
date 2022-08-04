![image](https://user-images.githubusercontent.com/99172259/182746144-e3ae6300-e622-46ef-a629-6b4b77e62388.png)


# CloudFront with S3 Hands on (SAA Course on Udemy by Stephane Maarek)



## Cloud Research

Storing your static content with S3 provides a lot of advantages. But to help optimize your application’s performance and security while effectively managing cost, we recommend that you also set up Amazon CloudFront to work with your S3 bucket to serve and protect the content. CloudFront is a content delivery network (CDN) service that delivers static and dynamic web content, video streams, and APIs around the world, securely and at scale. By design, delivering data out of CloudFront can be more cost effective than delivering it from S3 directly to your users. 

Source: https://aws.amazon.com/blogs/networking-and-content-delivery/amazon-s3-amazon-cloudfront-a-match-made-in-the-cloud/

## Try yourself

### Step 1 — Creating bucket with blocking all public access


### Step 2 — Creating distribution on CloudFront

On domain origin, choose the S3 bucket just created. And the name of the origin will be automatically filled in. But we can modify it. 

![image](https://user-images.githubusercontent.com/99172259/182746915-87836239-a688-4237-a740-aee903e7e588.png)


### Step 3 — Configure the bucket access and bucket policy

Make sure choose the following options so that the cloudfront can access the S3 and it is automatically change the bucket policy

![image](https://user-images.githubusercontent.com/99172259/182747422-c4ed9951-ff35-49f8-8cb2-6d06fcce3e58.png)

After that, click create and the bucket policy will automatically be updated

![image](https://user-images.githubusercontent.com/99172259/182749086-50155562-b4b2-413f-a399-eb921dabddeb.png)



## ☁️ Cloud Outcome

Using the website provided by the cloudfront we can access the file uploaded in the S3

![image](https://user-images.githubusercontent.com/99172259/182749300-dce29d54-c487-4094-8dea-a5287c828376.png)



## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1554839996397666304)
