

# Auto Scalling Group (A Course on Udemmy by Stephane Maarek)


## Cloud Research

<img src=https://user-images.githubusercontent.com/99172259/177274347-17e51c0c-4c80-4699-993d-6cb976667f1a.png width="500" height="300" />

How to create it

1. Create a template

<img src=https://user-images.githubusercontent.com/99172259/177274530-49833a2a-5095-4bc3-823c-dfab7fae52c6.png width="500" height="300" />

If you have not had a template, you can create a new one. Inside the template, you can set:

- Application and OS Images (Amazon Machine Image) 
- Instance type
- Key pair (login)
- Network settings
- and so on just like when you create a new instance

2. Launch the template

You can set the network (vpc and subnets). 

3. Advance Configuration

You can attach a load balancer

4. Configure group size and scaling policies

<img src=https://user-images.githubusercontent.com/99172259/177284676-f90a7e5a-8705-41d2-8cfa-9085df63b58a.png width="500" height="300" />

5. Add notifications (optional)

<img src=https://user-images.githubusercontent.com/99172259/177284895-28b2b5ee-ca14-4e16-a34d-493072044991.png width="500" height="300" />

6. Add tags (optional)

7. Review first and just click next and it will automatically launch a number of instances according to the limit you set


**The status of auto scaling group:**

![image](https://user-images.githubusercontent.com/99172259/177285461-b2d6edb5-a73b-48e3-b93b-6efc09576a07.png)


**Instances:**

![image](https://user-images.githubusercontent.com/99172259/177285557-b1d535fc-2f8f-41d0-8528-867067c68922.png)


**user data works for both instances:**

![image](https://user-images.githubusercontent.com/99172259/177285811-c85bee6f-268a-45bd-8eab-92116a50e1b3.png)

![image](https://user-images.githubusercontent.com/99172259/177286034-494f5430-f4ea-4472-b6c2-8c3a24d3452b.png)


**ELB: ALB  also works**

![image](https://user-images.githubusercontent.com/99172259/177286179-a1f87726-b178-45c8-aaa9-8209ac84bc67.png)


**When one instance is terminated a new instance will be launched:**


![image](https://user-images.githubusercontent.com/99172259/177286610-0769c083-be68-477d-b8f2-abc8a7332e8c.png)

**Deleting the auto scalling group will also delete all resources in it.**

![image](https://user-images.githubusercontent.com/99172259/177289024-15b4fa6b-0672-4e7c-8a0c-092503b18949.png)

### ASG - Policies

**Dynamic Scalling Policies**

- Target Tracking Scaling

use case : I want the average ASG CPU to stay at around 40%

- Simple/step scalling

When a cloudwatch alarm is trigerred (example CPU > 70%), then add 2 units

**Scheduled Actions**

Anticipate a scaling based on known usage patterns

Example : increase the min capacity to 10 at 5 pm on Fridays

**Predictive Scaling**

Continuesly forecast load and schedule scaling ahead


**ASG for Solutions Architects**

ASG Default Termination Policy (simplified version):

1. which AZ has the most numbers of instances
2. If there are multiple instances in the AZ, delete the oldest launch configuration

Lifecycle Hooks

By default as soon as an instance is launched in an ASG it's in service
you have the ability to perform extra steps before the instance goes in service and before the instance is terminated

## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1544265792518524928)
