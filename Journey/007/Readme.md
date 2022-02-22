# AWS CCP (Course on Udemmy by Stepahane Mareek): IAM Section

## Cloud Research

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

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
