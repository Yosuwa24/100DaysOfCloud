

# Containerization & Docker (An AWS SAA Course by Adrian Cantrill)

<img width="1924" alt="Containerization" src="https://user-images.githubusercontent.com/99172259/177656231-269ff3f4-6c85-4493-bc7d-25bf3905a6ea.png">


## Cloud Research

**Definition**

A container is a runnable instance of an image. You can create, start, stop, move, or delete a container using the Docker API or CLI. You can connect a container to one or more networks, attach storage to it, or even create a new image based on its current state.

By default, a container is relatively well isolated from other containers and its host machine. You can control how isolated a container’s network, storage, or other underlying subsystems are from other containers or from the host machine.

A container is defined by its image as well as any configuration options you provide to it when you create or start it. When a container is removed, any changes to its state that are not stored in persistent storage disappear.

[source](https://docs.docker.com/get-started/overview/)

[Docker Definition Explained in Bahasa Indonesia](https://www.youtube.com/watch?v=d2oOFasv0B4)

[Container explained in Bahasa Indonesia](https://www.youtube.com/watch?v=7tVt0JVkJy8)

## Installing Docker Engine on EC2 Instance Demo

1. **Create EC2 Instance using amazon linux AMI and t2.micro (Free tier) with public ip address**
2. **Installing docker on EC2**

- Run this command to install the engine

      sudo amazon-linux-extras install docker

- Start the docker engine

      sudo service docker start
      
- Enable your EC2 interact with the docker machine

      sudo usermod -a -G docker ec2-user

- Logout and login

       sudo su - ec2-user

3. **Build docker image**

- Run this command to create directory

      cd container
    
- create the container first. 

      docker build -t containerofcats .
    
- Create the image

      docker images --filter reference=containerofcats
    
4. **Run container from image**

       docker run -t -i -p 80:80 containerofcats
     
     

## Outcome

![image](https://user-images.githubusercontent.com/99172259/177659333-d3d6174d-7c6f-44a2-af31-5607b4701538.png)

    
    


## Social Proof

[Twitter](https://twitter.com/JoeSeven08/status/1544970371686084608)
