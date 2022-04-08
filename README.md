# Docker_config

## Introduction
This repository is used to install and configure an ELK stack. It interacts with the outside world through port 4444 syslog and 5044 with the beats software.

### Dependency:
docker

docker-compose

git

### Depedency Installation
#### docker
$ dnf config-manager --add-repo=https://download.docker.com/linux/centos/docker-ce.repo
$ yum install docker-ce -y
$ systemctl deamon-relaod
$ systemctl start docker.service
$systeemctl enable docker.service


$ yum install 



### Stack elk Installation
$ git clone https://github.com/BenjiMarchand/Docker_ELK

$ cd Docker_ELK 

$ docker-compose up -d

And that's it!
