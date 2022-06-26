

# Creating SNS Topic for S3 (Whizzlab Challenge)



## Cloud Research

- A company XYZ is deploying a new web application that helps customers to upload files to S3 Bucket. As a part of the infrastructure, the Administrator needs to be notified via Email whenever an object is put into their S3 bucket. Now your challenge is to setup the AWS architecture to perform this operation. 

Follow the below instructions to complete this challenge.

- Create a Standard Amazon SNS topic named mySnsChallengeTopic
- Add an Email subscription to that topic and verify it.
- Create a S3 bucket with a globally unique name.
- Update the Amazon SNS Topic Access Policy and add permission for S3 to publish messages to SNS Topic that you have created.
- Now, Create a S3 Notification Event named uploadObjectS3Event. 
- Select S3 Event type as Put.
- Select your SNS Topic as event Destination.
- Test the Configuration by uploading any sample PNG image file to S3 Bucket and see if you're notified. 


## ☁️ Cloud Outcome

<img src=https://user-images.githubusercontent.com/99172259/175828303-941fe85e-c533-496c-aa11-1f272a6f014c.png width="300" height="300" />


## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1540554568391868418)
