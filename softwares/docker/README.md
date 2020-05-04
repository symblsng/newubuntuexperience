
# Docker

## Install

    sudo apt-get install \
        apt-transport-https \
        ca-certificates \
        curl \
        gnupg-agent \
        software-properties-common
        
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
    sudo apt-key fingerprint 0EBFCD88
    
    
    sudo add-apt-repository \
        "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
            $(lsb_release -cs) \
            stable"
            
Due to the `focal` version is not released, so we use the `bionic` version(18.04)

    sudo add-apt-repository \
        "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
            bionic \
            stable"
         
    sudo apt-get update
    sudo apt-get install docker-ce docker-ce-cli containerd.io

## References

+ https://docs.docker.com/engine/install/ubuntu/
