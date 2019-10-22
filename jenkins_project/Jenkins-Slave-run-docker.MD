## Create project named "Docker application" and add below lines in build shell script section 
```sh


cd /home/jenkins-slave
git clone https://github.com/splunklearners/Jenkins-setup.git
cd ./Jenkins-setup/docker-compose
sudo docker-compose build
sudo docker-compose up -d



```



