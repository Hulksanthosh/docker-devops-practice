#Docker Image Commands

docker pull nginx
docker pull sonarqube
docker pull ubuntu
docker pull amazonlinux

docker images
docker rmi <image-id>
docker rmi -f <image-id>
docker rmi nginx
docker rmi ubuntu

#Docker Container Lifecycle Commands

docker run -td --name webserver1 -p 8080:80 nginx
docker run -td --name code-quality -p 9001:9000 sonarqube
docker run -it --name sample ubuntu /bin/bash
docker run -it --name webserver amazonlinux /bin/bash

docker ps
docker ps -a

docker stop <container-id>
docker start <container-id>
docker restart <container-id>
docker pause <container-id>
docker unpause <container-id>
docker rm <container-id>
docker rm -f <container-id>


#Docker Monitoring & Logs

docker stats
docker logs <container-id>
docker inspect <container-id>


docker exec -it <container-id> /bin/bash
