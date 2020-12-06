# Login without typing password

## Generate ssh key in client



    cd ~/
    mkdir .ssh
    ssh-keygen
    
    cd ~/.ssh
    cat id_rsa.pub

## Copy ssh key to server

    ssh-copy-id symbls@192.168.1.10