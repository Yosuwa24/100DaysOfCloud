

# Deploy web app on EKS part 2

## Cloud Research

### Error when installing libraries 

As the steps suggest, libraries should be installed by run this command **pip3 install -r requirements.txt** . Before doing that, the requirement.txt should be modified as it is suggested. But after that there is an error.


![error on libraries installation](https://user-images.githubusercontent.com/99172259/182505911-5ffe341d-d758-4d20-b456-bbc4403b73f0.JPG)

### Troubleshooting



- Install / update cdk cli & bootstraping cdk with aws account

Try to install cdk with the example version in the guide which is 1.121.0 . But the problem still occurs.

Source :https://docs.aws.amazon.com/cdk/v2/guide/cli.html



- Still got error > follow the suggesstion: removing the version on the requirement.txt 

Removing the version in the requirement as it is suggested by this [source](https://pip.pypa.io/en/latest/topics/dependency-resolution/#dealing-with-dependency-conflicts). But the result is still error.


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1553046215172177920)
