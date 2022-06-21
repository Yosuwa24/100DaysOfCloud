

# Cloudwatch Alarm - A Course on Learn Cantrill by Adrian Cantrill

## Cloud Research

Cloudwatch alarm can be used to warn us that something is not in accordance with our desired situation. For example, we want our instance to have cpu utilization not more than 15%. When it is equal or greater than 15% the alarm will be on. So, here are the steps to utilize cloudwatch alarm

- Create an EC2 instance
- t2.micro
- ensure its set to the default VPC and has a public IP
- Optionally enable detailed monitoring
- Connect to the instance and install Extras package and stress
- Install stress (commands listed in code sample below)
- Create an alarm based on the CPU Utilisation of the created instance
- Threshold greater than 15%
- Run stress 'stress -c 2'
- Wait for alarm to .. alarm
- use ctrl + c to cancel stress




## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1529120055505526784)
