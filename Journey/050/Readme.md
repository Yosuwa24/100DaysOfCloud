

# NAT & PAT - A Course on Learn Cantrill by Adrian Cantrill

## Cloud Research

**Network Address Translation (NAT)**

A private IP should be translated into a public IP in order that it can communicate with the internet. The NAT device will be needed to do the translation. NAT are devided into two categories:
1.  Static NAT
  1 private ip translated into one permanent public ip
2. Dynamic NAT
Public ip allocations are temporary allocation from a public ip pool. Multiple private ip can use the same public ip. If the public IP pool is exhausted, external access can fail.

**Port Address Translation (PAT)**

When using dynamic NAT, it will also translate the port source within the NAT gateway. 

![PAT (1)](https://user-images.githubusercontent.com/99172259/168200335-802c72cc-3198-4899-8177-f0647a3f34f2.jpg)

## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1524942443594280961)
