# nginx docker conatiner change if user is not ubuntu

```
mkdir -p /var/lib/docker/nginx/content
cp -rp /home/ubuntu/team7-docker/nginx/nginx.conf /var/lib/docker/nginx
docker run --name nginx -v /var/lib/docker-data/nginx:/etc/nginx:rw -d nginx
```
