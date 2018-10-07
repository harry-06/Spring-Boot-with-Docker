# Spring-Boot-with-Docker
Sample Spring Boot application in Docker


Steps
======
1. Download and install Docker from official docker website www.docker.com( as per your OS)
2. Start the Docker engine from installation.
3. Go to Spring.io website and create simple spring boot application with single rest end point.
4. Create DockerFile (Find sample in this repository.Note :This is required to build Docker image)
5. Build Docker image using command ==>Docker build -f Dockerfile -t docker-spring-boot .
   (note:1. DockerFile -->D should be uppercase . 2.Docker-spring-boot->Docker container name, 3) Needs to mention the
   files directory and if its in the current directory give Dot(.))
 6. Check if the docker image is created successfully using command ==> docker images
 7.Run Docker image using command ==> docker run -p 8085:8085 docker-spring-boot
 8.if required change the application port using application.properties file( springboot has embedded Tomcat server 
 which by default starts in port 8080)
 9.Go to browser and give url : http:localhost:8085/rest/docker/hello
 
 
