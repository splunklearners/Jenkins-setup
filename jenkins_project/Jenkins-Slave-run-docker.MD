Below lines needs to add in build script of jenkins

cd /home/jenkins-slave
git clone https://github.com/splunklearners/Jenkins-setup.git
cd ./Jenkins-setup/docker-compose
sudo docker-compose build
sudo docker-compose up -d

