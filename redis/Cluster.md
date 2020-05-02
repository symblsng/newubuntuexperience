# Cluster

## References

https://redis.io/topics/cluster-tutorial

## The Minimal Cluster

The minimal `redis.conf` file:

    port 7000
    cluster-enabled yes
    cluster-config-file nodes.conf
    cluster-node-timeout 5000
    appendonly yes

Make several directories:

    mkdir cluster-test
    cd cluster-test
    mkdir 7000 7001 7002 7003 7004 7005
    
Copy six redis.conf to six directories and modify the port

Copy the compiled `redis-server` to the current directory:

    cd 7000
    ../redis-server ./redis.conf
    
Then A Server started.

### White Space For Pause

Install ruby:

    sudo apt install ruby
    
And then:
    
    gem install redis
