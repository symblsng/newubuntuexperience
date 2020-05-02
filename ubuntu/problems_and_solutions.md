# Problems And Solutions

My Ubuntu Version is Ubuntu Kylin Desktop 16.04

## Mouse and Keyboard don't work

    sudo apt-get dist-upgrade     # Maybe it will work? I haven't try

## Wired connection doesn't work

I have not solutions now. You can try to run the following:

    sudo service network-manager restart
    
then connect to your wired network again.

and maybe the following command affects:

    sudo apt install ethtool
    sudo ethtool eth0
