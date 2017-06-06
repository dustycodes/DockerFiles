#Jenkins
## install docker
sudo apt-get -y install docker.io
sudo su

## create jenkins user
sudo su
useradd -u 1008 -g rex -s /bin/bash -m jenkins
su - jenkins
ssh-keygen -b 2048
ssh-copy-id -i ~/.ssh/id_rsa.pub jenkins@gitserver

## Run
docker build -t jenkins-image .
docker run --name jenkins-image -d -t -p 8023:8080 -e TZ="America/Denver" -v /opt/jenkins:/var/jenkins_home -v /home/rex/work:/work jenkins
