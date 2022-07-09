
# ECS - Hands On

## Cloud Research : Running the Task Definition behind a Load Balancer

### Creating ECS Cluster

1. Create name of the cluster, setting the networking

<img src=https://user-images.githubusercontent.com/99172259/178082494-5a4edb40-c8e4-49f1-8570-b68d735e33d3.png height="400" widht="500" />

2.Configure the infrastructure. The fargate will automatically be ticked.

<img src=https://user-images.githubusercontent.com/99172259/178082542-5ed5a401-56e6-40d0-80cd-8f9efe392c89.png height="400" widht="500" />

3. Monitoring and tags are optional. Then, click create.

<img src=https://user-images.githubusercontent.com/99172259/178082575-24973fc7-8233-4247-92cf-f859ba0e0ed8.png height="200" widht="600" />

After creation

- Check the ASG and the instance on EC2 menu

![image](https://user-images.githubusercontent.com/99172259/178082736-04099c9e-bc05-4c66-99a2-210d3387e8b3.png)

- On ECS menu, you can click the cluster you have created and check the infrastructure tab.

<img src=https://user-images.githubusercontent.com/99172259/178082974-4cf24aba-54f6-44b2-9ed3-c9984c5dff1a.png height="200" widht="600" />


### Creating Task Definition


1. Fill in the configuration. Here I use nginxdemo/hello for the web server. You can find it on website.

<img src=https://user-images.githubusercontent.com/99172259/178083746-a2b225c4-e6c3-45d5-a321-261b206c04db.png height="400" width="500" />


**nginxdemo/hello website**

<img src=https://user-images.githubusercontent.com/99172259/178083816-2b8754ee-29b7-4353-874a-3fdcda0ec24f.png height="200" widht="600" />

2. Configure environment, storage, monitoring, and tags

- Environment

<img src=https://user-images.githubusercontent.com/99172259/178083992-71d77179-5512-4406-91dc-31daf4bde6cb.png height="400" widht="500" />

- storage, monitoring, and tags

Leave it as default. For the monitoring, I have turned off use log collection.


### Creating Security Groups for ALB & Task Definition

1. Create a new security group for ALB allowing port 80 accessed from anywhere IPv4 and IPv6.

<img src=https://user-images.githubusercontent.com/99172259/178084332-fac98ce3-427d-42c9-8625-4b4f9202ddb2.png height="200" widht="600" />

2. Create a new security group for the task definition allowing the inbound from alb sg from all tcp.

<img src=https://user-images.githubusercontent.com/99172259/178084561-c2dd0f80-73a8-4c2a-a60e-befbda1a73e6.png height="200" widht="600" />


### Running a Service

1. Back to ECS, click your cluster, service and deploy

<img src=https://user-images.githubusercontent.com/99172259/178084862-adef4961-0314-4b8e-acca-8cf96a92c10d.png height="200" widht="600" />

2. Configure the deployment

- For the application type, since I implemented web server so I chose service
- Family belongs to the task definition I just created
- We can how many desired tasks. It means if we set 2 desired task, later there will be 2 web servers

<img src=https://user-images.githubusercontent.com/99172259/178084959-e95186ef-2a7a-4bf9-a9dd-3b34e4300ccf.png height="400" widht="500" />

3. Create ALB and target group

<img src=https://user-images.githubusercontent.com/99172259/178085146-b64f54a0-1a5f-40ff-9e8f-399efdc70bc2.png height="400" widht="500" />

4. Configure the networking and choose the sec group for the ALB

<img src=https://user-images.githubusercontent.com/99172259/178085207-abc06bf8-7280-4dc9-a105-f9d3d858a5cd.png height="400" widht="500" />

5. Check the health

<img src=https://user-images.githubusercontent.com/99172259/178085545-8a1e4d2f-1a80-4112-9f67-d1a5fbe6f3bc.png height="200" widht="600" />

6. Open the URL from the Load Balancer

![image](https://user-images.githubusercontent.com/99172259/178085610-8c01f05d-d297-445c-8e92-bf7886fb027d.png)



### Scalling our Service

1. Click on edit serviec

<img src=https://user-images.githubusercontent.com/99172259/178085693-6069a208-e638-4cc5-b6c3-b2ba43bae3f7.png height="200" widht="600" />

2 Update the task

<img src=https://user-images.githubusercontent.com/99172259/178085727-5a5a364a-0e45-4c11-a6b1-60b1364ede9e.png height="400" widht="500" />


<img src=https://user-images.githubusercontent.com/99172259/178085774-1781a49e-091c-4ac7-b5b8-a8301400f4e7.png height="400" widht="500" />

3. Check the ALB 

<img src=https://user-images.githubusercontent.com/99172259/178085795-0d9a1a39-cf3b-4a36-b55e-64fc8d064fe3.png height="400" widht="500" />

<img src=https://user-images.githubusercontent.com/99172259/178085803-fb2e0560-f3cb-4c21-8c2a-b530df208b63.png height="400" widht="500" />

4. Now set it to 0

<img src=https://user-images.githubusercontent.com/99172259/178085817-bd5354cf-545f-4861-b1d5-69d38396536e.png height="400" widht="500" />

## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1545589749574152192)
