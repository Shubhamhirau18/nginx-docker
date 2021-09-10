## Prerequisite 

## Make Sure Port 80,8001,8002 Not Already In Use on Host Machine

## Tested On Docker Version
- Docker version 20.10.8
- docker-compose version 1.29.2 

## Run Docker Compose UP Command to Spin Up Stack
$ docker-compose up -d

## Access Url : It will be accessible on Your Host IP, Please replace with Your Host Machine IP
- http://<Host-IP>/

## Outcome : It Will Load Balance Between two Python Application Running on Port 8001,8002
## Load Blanacing Algorithm : Round Robin
