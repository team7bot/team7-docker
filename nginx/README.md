# nginx docker conatiner change if user is not ubuntu

```
mkdir -p /var/lib/docker-data/nginx
cp -rp /home/ubuntu/team7-docker/nginx/* /var/lib/docker-data/nginx
docker run --name nginx -v /var/lib/docker-data/nginx:/etc/nginx:rw -d nginx
```
