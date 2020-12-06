# Not Must Use

[Others](server/mysql/common.md)

## Nat123

    sudo apt install mono-complete
    cd ~ && mkdir nat123 && cd nat123
    wget http://www.nat123.com/down/nat123linux.tar.gz
    tar -zxvf nat123linux.tar.gz


## Jenkins

    docker pull jenkins/jenkins:lts
    docker run -u root -d -p 10001:8080 -p 50000:50000 -v jenkins-data:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock --name jenkins jenkins/jenkins:lts
    
### Run jenkins automatically after startup
    
    docker update --restart on-failure:10 jenkins

    
[References](./softwares/jenkins/README.md)    


