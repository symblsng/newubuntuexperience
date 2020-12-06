# Servers

## ssh

[README](./ssh/README.md)

## Init

sudo su

    apt update
    apt upgrade

## Init Folder
    
    mkdir /home/symbls/apps
    mkdir /home/symbls/envs

## Nginx,Git,Maven

    sudo apt install -y nginx

    sudo apt install -y git

    sudo apt install -y maven

## Mysql Server

    sudo apt install -y mysql-server

Reference:

+ https://dev.mysql.com/doc/mysql-apt-repo-quick-guide/en/#repo-qp-apt-install-from-source)

[Create New User](./mysql/common.md)

[Allow being visiting by remote user](./mysql/common.md)

## Docker

[Docker](./docker/README.md)

## Docker Accelerator

[Ali accelerator](https://cr.console.aliyun.com/cn-hangzhou/instances/mirrors)

## Jre

    sudo apt install -y openjdk-14-jre

Reference:
+ https://developer.aliyun.com/packageSearch?word=jre

## Jenkins

    docker pull jenkins/jenkins:lts
    docker run -u root -d -p 11001:8080 -p 11002:50000 -v jenkins-data:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock --name jenkins jenkins/jenkins:lts

Run jenkins automatically after startup

    docker update --restart on-failure:10 jenkins

Reference:
+ https://jenkins.io/

[Install docker in jenkins container](./jenkins/README.md)

[Login without typing password](./ssh_key/git_ssh_key.md)