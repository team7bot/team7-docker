# jenkins build
```
cd /home/ubuntu/team7-docker/jenkins
docker build -t myjenkins .
docker run --name jenkins -h jenkins -p 1080:8080 -p 50000:50000  -d myjenkins
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```

go to browser http://server:1080
enter the password shown by last docker command
add the community plugins
