

# Build an Application Using a NoSQL Key-Value Data Store Part 1



## Prerequisite

- An AWS account: If you don't already have one, follow the Setting Up Your Environment getting started guide for a quick overview.
- An installed version of the AWS Python SDK via pip install boto3

## Cloud Research

In this tutorial, you will create a bookstore application that showcases a product catalog. Products typically contain unique identifiers and attributes such as descriptions, quantities, locations, and prices. The method for retrieving these types of attributes (specifically, the access pattern) is often a key-value lookup based on the product’s unique identifier. This means that an application can retrieve these other attributes when a product’s unique identifier is provided.

![image](https://user-images.githubusercontent.com/99172259/180802947-0d6a8880-17a2-4e2e-811f-539b056f9ee4.png)


The complete guide can be seen [here](https://aws.amazon.com/getting-started/guides/build-an-application-using-a-no-sql-key-value-data-store/?pg=nosql)

Before doing the steps above, install boto3 first. You can read the full guideline here:

https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html


## Try yourself

### Step 1 — Installing Python on Command Prompt

https://www.python.org/downloads/

### Step 2 - Install Boto3

![image](https://user-images.githubusercontent.com/99172259/180805101-0202ba7d-1055-4967-94c1-fac6449e047c.png)


### Step 3 — Using the AWS Common Runtime (CRT)

Run these commands on the command prompt

     pip install boto3[crt]
  
To revert to the non-CRT version of Boto3, use this command:
  
      pip uninstall awscrt

If you need to re-enable CRT, reinstall boto3[crt] to ensure you get a compatible version of awscrt:
     
     pip install boto3[crt]
     
     
### Step 4 — Configuration

run command

    aws configure
    
    
### Step 4 — Using Boto3

**Login into python**

     pyhton

**Run this command**

     import boto3

Now let see amazon s3 bucket in our S3

    s3 = boto3.resource('s3')

Then this

    for bucket in s3.buckets.all():
      print(bucket.name)

## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1551231951042129920)
