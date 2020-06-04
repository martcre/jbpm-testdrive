# jbpm-testdrive

## Setup
  - Install Docker for Windows https://docs.docker.com/docker-for-windows/install/
  - or for Mac https://docs.docker.com/docker-for-mac/install/
  - then Pull JBPM Full from Docker Hub https://hub.docker.com/r/jboss/jbpm-server-full with command ```docker pull jboss/jbpm-server-full```
## Usage
  - Start the docker image with ´´´docker run -p 8080:8080 -p 8001:8001 -d --name jbpm-server-full jboss/jbpm-server-full:latest´´´
  - Open http://localhost:8080/business-central in your Browser
  - Test User:
  
```
  USER        PASSWORD    ROLE
*************************************************
wbadmin     wbadmin     admin,analyst,user,process-admin,kie-server
krisv       krisv       admin,analyst,user,process-admin,kie-server
john        john        analyst,Accounting,PM,kie-server
sales-rep   sales-rep   analyst,sales,kie-server
katy        katy        analyst,HR,kie-server
jack        jack        analyst,IT,kie-server
```
  - Stop the Docker image with ´´´docker stop jbpm-server-full´´´