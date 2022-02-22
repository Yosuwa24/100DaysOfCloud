# AWS CCP (Course on Udemmy by Stepahane Mareek): IAM Section & Aguna Course : Virtual Machine Fundamental

## Cloud Research

## AWS-CCP

**Password and authentication for IAM Users**

The root may configure the password policies like how many characters, alphanumeric and so on. And to make it more secure, the IAM users may also activate MFA (Multi Factor Authentication) when he/she login. Here are supported MFA by AWS:
1. Virtual MFA device
- Google authenticator (phone only)
- Authy (Multi-device)

2. Universal 2nd factor (U2F) Security key
- Yubikey by Yubico (3rd party)

3. Hardware Key Fob MFA Device

- Provided by Gemalto (3rd party)

4. Hardware Key Fob MFA Device for AWS GovCloud (US)

- Provided by SurePassID (3rd party)

**How users can access AWS**
1. AWS Management Console (password + MFA)
2. AWS Command Line Interface (CLI) : protected by access keys
- Enables you to interact with AWS using commands
- Need to install CLI from AWS : AWSCLIV2 
- After that, just open your command prompt and check if it is running by type aws --version
- if the reply 

aws-cli/2.4.19 Python/3.8.8 Windows/10 exe/AMD64 prompt/off

it is working

- to login, you can type aws configure and later you need to input access key id, password and region name

3. AWS Software Developer Kit (SDK) - for code : protected by access keys 

It is basically for programming using some code languages and aws sdk can be embedded in your application

**IAM Roles for Services**
- Policies for services

**IAM Security Tools**
 - Credentials reports
it reports the user security information like when it is created, the password, MFA active or not and so on

- IAM Access Advisor
Show the service permissions granted to a user and when it was last accessed

## Aguna Course : Virtual Machine Fundamental

I take this session since it is necessary to take before discussing EC2 on AWS.

**Definition of Virtual Machine**

It is a virtual computer that can operate without any physical hardware (CPU, memory, NIC, disk). To create virtual machine we still need computer and install hypervisor. One of the hypervisors is esx server.  

**Types of Virtual Machine Architecture**

1. Bare-Metal 
Hardware - Hypervisor - Guest OS VM

Hypervisor used: 

VMwareesxi (licensed)

Proxmox : Free

Use case: Data center servers

2. Hosted Architecture
Hardware - Host OS - Hypervisor - Guest OS VM

Hypervisor used: 

vmware (licensed)

virtualbox (free)

Use case : Laptop or computer for virtual machine testing'

**Useful source for learning before learning EC2 on AWS CCP**

AWS Power Hour: Cloud Practitioner | S2 E2 (Blaine) | Compute & Network

https://www.twitch.tv/aws/video/772551330

## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1496090921808838662)
