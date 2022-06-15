

# S3 Pre-Signed URL Demo, S3 Select & Glacier Select


## Cloud Research

### Pre-Signed URL Demo

There are two ways to generate pre-signed URL:

**Using S3 Console**

The simplest way! 

- Click on the object you want to
- Click on object action
- Choose share with presigned url and it will generate the url

<img src=https://user-images.githubusercontent.com/99172259/173767402-4cd8a052-4408-4916-b505-32c929bcf1ca.png widht="200" height="300" />

**Using AWS CLI**

- Click on the AWS CLI

![image](https://user-images.githubusercontent.com/99172259/173768848-e98897e5-5840-49bc-8f92-fd93d43bfa67.png)

- run this command
 
 aws s3 presign <s3 object uri> --expires-in <the time limit in seconds>
  
  example
  
  aws s3 presign s3://awsbucketforurlpredesign/all5.jpg --expires-in 180
  
  note: 
  - name your uploaded file without uppercase and space. I got an error when try this method using AWS CLI
  
  ![image](https://user-images.githubusercontent.com/99172259/173769684-20a6b5df-5094-45ac-b6a8-717a72315dc9.png)


- If you do not have access to the bucket due to the IAM policy disabling you to access S3, after you generate the pre-signed url in the AWS Cloudshell, the file becomes still unaccessable. It is because the pre-signed url access policy is inheritted from the user IAM policy.
  
### S3 Select & Glacier Select
  
- It is used to filter data by using SQL like statement from the S3 Side. S3 will share only the data that we need.
- The data can be in the form of CSV, JSON, Parquet, BZIP2 compression for CSV and JSON
  
### S3 Events Notification
- S3 can notify us activities inside S3 such as uploading object, deleting object and so on
- The events can be filterred such as we want only to be notified if file in the format of jpg is uploaded
- It can be integrated with SNS, SQS, Lambda and eventbridge
  


## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
