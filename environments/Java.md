# Java

## Config Java Environment

1.Edit `/etc/profile` using `sudo vi /etc/profile`:

    export JAVA_HOME=/home/symblx/envs/jdk-11.0.7
    export PATH=$JAVA_HOME/bin:$PATH
    export CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar

2.Run the command `source /etc/profile` to make your configuratioon available.

3.Check the environment is available with `java -version`, the output should be like

    java version "11.0.7" 2020-04-14 LTS
    Java(TM) SE Runtime Environment 18.9 (build 11.0.7+8-LTS)
    Java HotSpot(TM) 64-Bit Server VM 18.9 (build 11.0.7+8-LTS, mixed mode)

