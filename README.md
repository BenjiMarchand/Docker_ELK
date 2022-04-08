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

$ systemctl start docker.service

$ systemctl daemon-reload

$ systemctl enable docker.service

#### docker-compose
$ curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

$ chmod +x /usr/local/bin/docker-compose

#### git
$ yum install git

=====================================================================================================

### Stack ELK Installation
$ mkdir /data

$mkdir /data/elastic_data

$chmod 777 /data/ -R

$ git clone https://github.com/BenjiMarchand/Docker_ELK

$ cd Docker_ELK 

$ docker-compose up -d

##And that's it!
