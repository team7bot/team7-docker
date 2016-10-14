# nginx docker conatiner change if user is not ubuntu

```
mkdir -p /var/lib/docker-data/nginx/content
cp -rp /home/ubuntu/team7-docker/nginx/nginx.conf /var/lib/docker-data/nginx
docker run --name nginx -v /var/lib/docker-data/nginx/content:/usr/share/nginx/html -v /var/lib/docker-data/nginx/config/nginx.conf:/etc/nginx/nginx.conf -d nginx
```
