# Not Must Use

    sudo apt install openssh-server

    sudo apt-get install mysql-server

## Nat123

    sudo apt install mono-complete
    cd ~ && mkdir nat123 && cd nat123
    wget http://www.nat123.com/down/nat123linux.tar.gz
    tar -zxvf nat123linux.tar.gz

## Nginx 

    sudo apt install nginx
    
## Docker

[Docker](./softwares/docker/README.md)

## Jenkins

    wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
    
edit the file using `vi /etc/apt/sources.list` and add the following line in the end of the file(The add-apt-repository is not effective here) 

    deb https://pkg.jenkins.io/debian-stable binary/

Add then

    sudo apt-get update
    
    sudo apt-get install jenkins
    
[References](./softwares/jenkins/README.md)    

## Useless

    sudo apt install openjdk-11-jre-headless
