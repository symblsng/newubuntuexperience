# Common Command

## Modify the crontask

Shutdown your computer daily:

    sudo vi /etc/crontab
  
and add the following:

    55 23   * * *   root    shutdown -h now

and then run the following command:
  
    /etc/init.d/cron reload
