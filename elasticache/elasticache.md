# Elasticache AWS
## Redis
inspiration: https://github.com/widdix/aws-cf-templates/blob/master/state/elasticache-redis.yaml

```
sudo amazon-linux-extras install epel -y
sudo yum install gcc jemalloc-devel openssl-devel tcl tcl-devel -y
sudo wget http://download.redis.io/redis-stable.tar.gz
sudo tar xvzf redis-stable.tar.gz
cd redis-stable
sudo make BUILD_TLS=yes
```
Note:
If the cluster you are connecting to isn't encrypted, you don't need the Build_TLS=yes option.
connect to redis:
` src/redis-cli -h cluster-endpoint -c -p port number ` 