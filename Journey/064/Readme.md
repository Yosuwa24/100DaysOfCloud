
![image](https://user-images.githubusercontent.com/99172259/172757301-a7d37f77-4a60-4c07-b6fb-02afb60f1d47.png)



# 101 Encryption


## Introduction

It is based on Adrian Cantrill and Stephane Maarek courses. 


## Cloud Research

### Definition

Basically, when you want to improve the security on your data, especially when you want to give it to someone else you must encrpyt the data. The data that is important for us such as credit card numbers, passwords, etc. The data encruption have four components:

- plain text
- algorithm
- key
- chipertext

![image](https://user-images.githubusercontent.com/99172259/172758033-4218c2eb-f7b4-4cc6-944d-e5aa208a7898.png)

pic source : https://steemit.com/programming/@alfarisi/proses-enkripsi-data-plain-text-encryption-algorithms-encrypt-data-a-plain-text-java-source-code


### Terms

Symmetric : a type of encryption where only one key (a secret key) is used to both encrypt and decrypt electronic data. The entities communicating via symmetric encryption must exchange the key so that it can be used in the decryption process

https://www.cryptomathic.com/news-events/blog/symmetric-key-encryption-why-where-and-how-its-used-in-banking#:~:text=Symmetric%20encryption%20is%20a%20type,used%20in%20the%20decryption%20process.

Assymmetric : Asymmetric cryptography, also known as public-key cryptography, is a process that uses a pair of related keys -- one public key and one private key -- to encrypt and decrypt a message and protect it from unauthorized access or use.

https://www.techtarget.com/searchsecurity/definition/asymmetric-cryptography


Cryptographic : Encryption and decryption process

### KMS (Key Management Service)


It is an AWS service to create key for our data. It is not free! it cost $1 per month for each key you create.

AWS Key Management Service (AWS KMS) makes it easy for you to create and manage cryptographic keys and control their use across a wide range of AWS services and in your applications. 

**How it works?**

AWS KMS helps you centrally manage and securely store your keys. You can generate keys in AWS KMS or import them from your own key management infrastructure. You can submit data directly to AWS KMS to be encrypted, or decrypted. Other AWS services can use your keys on your behalf to protect data encryption keys that they use to protect your data.

Your keys never leave AWS KMS and you are always in control of your keys. You can set usage policies that determine which users can use your keys and what actions they can perform. All requests to use these keys are logged in AWS CloudTrail so that you can track who used which key, how and when.

<img src=https://user-images.githubusercontent.com/99172259/172759012-a7d00200-78c0-467a-86f7-0d2f8cb0a43e.png width="700" height="450" />


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1534540992396767233)
