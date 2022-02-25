# Elastic Block Storage & Amazon Machine Image (CCP Course on Udemy by Stephane Mareek) 

## Prerequisite

It is better to know cloud storage types. To comprehend that, you can check out this [youtube video](https://www.youtube.com/watch?v=3r9RGJ0_Bls)

## Cloud Research

**EBS**

Definition

It is simply a network drive attached to an instance. It can be attached to another instance in the same availability zone. To move the volume into another availability zone weh have to create snapshot. 

Volume  : the data inside the instance (from my point of view)

Snapshot : backup of volume

Some practices you can do

- How to create additional volumes on the same availability zone
- Terminating an instance and see whether the volume still there or not
- How to create snapshot (backup) from a volume
- How to create volume from a snapshot and attach it to other region


**AMI**

Definition

An AMI is a template that contains the software configuration (operating system, application server, and applications) required to launch your instance. You can select an AMI provided by AWS, our user community, or the AWS Marketplace; or you can select one of your own AMIs.

Practice

- Creating AMI after creating instance
- Creating instance using existing AMI


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1497277382168018944)
