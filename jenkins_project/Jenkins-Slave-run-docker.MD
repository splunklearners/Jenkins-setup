## Create project named "Docker application" and add below lines in build shell script section 
```sh


cd /home/jenkins-slave/workspace/dockerdeploy/docker-compose
sudo docker-compose build
sudo docker-compose up -d

```
##Once docker is up and running as per docker compose file, your application is running on port 9001, you need to port 9001 in aws security group. and you can access application from browser - http://yourslaveip:9001


