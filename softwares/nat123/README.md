## Run

    mono nat123linux.sh

## Instructions

+ http://www.nat123.com/pages_17_600.jsp

## Run While Startup

    vi /etc/rc.local
    
Content: 

    #!/bin/sh -e
    #
    # rc.local
    #
    # This script is executed at the end of each multiuser runlevel.
    # Make sure that the script will "exit 0" on success or any other
    # value on error.
    #
    # In order to enable or disable this script just change the execution
    # bits.
    #
    # By default this script does nothing.
    
    cd /home/symblx/apps/nat123
    mono nat123linux.sh service &
    exit 0
    
Grant permission

    chmod 777 /etc/rc.local
    
### Other

In Ubuntu 20, the rc.local is not suggested.
    
