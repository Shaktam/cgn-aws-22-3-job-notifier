```
Steps to run container on ec2 instance
Push container to registry ( For example docker Hub)
Register for account if you have not done it
 2. Create a repository if you have not done it
3. build container with tag from repository
(If you have m1 use docker buildx)
 docker buildx build --platform linux/amd64 . -t fabianschmauder/job-notifier-cgn-aws-22-3:0.3
Login to docker hub
docker login
push your container
docker push fabianschmauder/job-notifier-cgn-aws-22-3:0.3

```

## in VS Code
cd api-server
 1215  docker login
 1216  docker buildx build --platform linux/amd64 . -t shaktam/job_notifier-cgn-aws-22-3:0.2
 1217  docker buildx build --platform linux/amd64 . -t shaktam/job_notifier-cgn-aws-22-3:0.2
 1218  docker push shaktam/job_notifier-cgn-aws-22-3:0.2
 1219  sudo docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.2
 1220  docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.2
 1221  docker buildx build --platform linux/amd64 . -t shaktam/job_notifier-cgn-aws-22-3:0.3
 1222  docker push shaktam/job_notifier-cgn-aws-22-3:0.3
 1223  docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.
 

 ```
 *  Run on ec2:
*   ssh into instance
*   install docker (https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-container-image.html)
run docker  container with run command and link to your docker hub repo
docs.aws.amazon.comdocs.aws.amazon.com
Creating a container image for use on Amazon ECS - Amazon Elastic Container Service
Amazon ECS uses Docker images in task definitions to launch containers. Docker is a technology that provides the tools for you to build, run, test, and deploy distributed applications in containers. Docker provides a walkthrough on deploying containers on Amazon ECS. For more information, see
```

create ec2 Instance with vpc,subnet,route table,securitygroup, internet gateway
connect to local maching using ssh
## terminal 

   15  docker
   16  sudo yum update -y
   17  sudo amazon-linux-extras install docker
   18  sudo service docker start
   19  sudo systemctl enable docker
   20  sudo usermod -a -G docker ec2-user
   21  sudo docker ps
   26  docker buildx build --platform linux/amd64 . -t shaktam/job_notifier-cgn-aws-22-3:0.2
   28  sudo docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.2
   29  docker ps -a
   30  docker rm 6ee75f84ef1b
   31  docker ps -a
   32  docker rm 5923df47e045
   33  docker ps
   34  docker ps -a
   35  sudo docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.2
   36  docker ps -a
   37  sudo docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.2
   38  sudo docker ps
   39  sudo docker ps -a
   40  history
   41  sudo docker run -p 80:80 -d shaktam/job_notifier-cgn-aws-22-3:0.3
   42  sudo docker ps
   43  history

 