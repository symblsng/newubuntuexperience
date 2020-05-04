#

This is not suggested for now. The reason is:

+ Error occurs while the plugins cannot be downloaded for several times.
+ Not convenient for configuration
+ Other reasons?

## Installation

    wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
    
edit the file using `vi /etc/apt/sources.list` and add the following line in the end of the file(The add-apt-repository is not effective here) 

    deb https://pkg.jenkins.io/debian-stable binary/

Add then

    sudo apt-get update
    
    sudo apt-get install jenkins

## Remove 

    sudo apt remove jenkins


## Installation References

+ https://pkg.jenkins.io/debian-stable/
