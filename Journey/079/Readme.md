

# ELB : SSL Certificate & Connection Drainibg (A Course on Udemy by Stephane Maarek)


## Cloud Research

### SSL Certificate

![image](https://user-images.githubusercontent.com/99172259/177186918-69294496-71bc-4d4f-8a59-618ba20800ac.png)

SNI solves the problem of loading multiple SSL certificates onto one web server (to serve multiple websites)

Only works for ALB & NLB (newer generation), CloudFront

### Connection Draining/Deregistration Delay

Time to complete “in-flight requests” while the  instance is de-registering or unhealthy

Stops sending new requests to the EC2 instance which is de-registering


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1543987510606712832)
