# Jenkins

## Problems

If it is stuck after input the password:

+ try update the url in `Update Site` in the website `http://your_jenkins_domain/pluginManager/advanced` to

    http://mirror.xmission.com/jenkins/updates/update-center.json

+ and set the connectionCheckUrl from `http://www.google.com/` to `http://www.baidu.com/` in the file `$JENKINS_HOME/updates/default.json`   -e.g. `/var/jenkins_home/updates/default.json`

