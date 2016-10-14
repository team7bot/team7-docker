# jenkins build
```
cd /home/ubuntu/team7-docker/jenkins
docker build -t myjenkins .
docker run --name jenkins -h jenkins -p 1080:8080 -p 50000:50000  -d myjenkins
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
```

Configure jenkins
- go to browser http://server:1080
- enter the password shown by last docker command
- add the community plugins
- create first admin user
-- user: team7bot
-- pwd: team7bot!

Job Import Plugin import all jobs 
-	http://rajeev1689.ddns.me:10098/
-	User raj
-	Pwd Happy1689

Open team7-mail config
-	update git password
-	user team7bot
-	pwd team7bot!

Do a team7-mail build

