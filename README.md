# Learning Management System

## REACT JS - Presentation tier
## NODE JS - Application tier
## POSTGRES - Data tier

**Install Docker**
> docker
> curl -fsSL https://get.docker.com -o get-docker.sh
> sh get-docker.sh
> docker
 
**Install Sonarqube**
> sudo ss -ntpl
> sudo docker container run -dt --name sonarqube -p 9000:9000 sonarqube
> sudo ss -ntpl
>
**Solar analysis**

cd ~/lms/webapp

sudo docker run  --rm -e SONAR_HOST_URL=http://54.177.219.62:9000 -e SONAR_TOKEN=sqp_a5fbf4ddee2592601b714fcc088a983e738d9213  -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms
