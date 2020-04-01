Lesson 3 - Containers - Exercise
The exercises in this lesson are an extension of the exercises you have already done in the previous lesson - "Independent Development". We will use the same "Udagram" project, and convert the monolithic architecture into microservices running in separate containers. We will use Docker to run our application. First, we start with packing our application and afterward we will create an Nginx proxy. Finally, we will use docker-compose to deploy our complete application.

Dependencies
We have already described the instructions at https://github.com/udacity/nd9990-c3-microservices-v1/blob/master/lesson-2-Independent-Development/exercises/README.md to get the following installed on your system.

Installing Node and NPM
Installing Ionic Cli
AWS RDS - PostgreSQL instance, Postbird tool, and an S3 bucket
Docker Desktop - macOS, Windows 10 64-bit: Pro, Enterprise, or Education, Windows 10 64-bit Home. You can find installation instructions for other operating systems at: https://docs.docker.com/install/
Once you have Docker installed, open a terminal and run:

docker run alpine echo hello world
Exercise Instructions
Task 1 - Clone the project GitHub repository (if not already)
Clone the course repo and stay on the master branch.

git clone https://github.com/udacity/nd9990-c3-microservices-v1
cd nd9990-c3-microservices-v1/
git branch
Navigate to the /lesson-3-Container/exercises/ directory, where you would find the following sub-folders for each component of the project, as follows:

udacity-c3-frontend - For Ionic client web application, which consumes the RestAPI Backend
udacity-c3-restapi-feed - For "feed" microservice
udacity-c3-restapi-user - For "user" microservice
udacity-c3-deployment/docker - For running the Nginx as a reverse-proxy server It will be helpful if you download and install the Visual Studio Code editor. Follow the instructions as available in the classroom.
Task 2 - Create Docker Images for our application
Create a Dockerfile for all the three services in the respective directories. The three services are - "feed", "user", and "frontend".
Use the Dockerfile to create the corresponding images for all the three services.
Task 3 - Create Docker Image for Nginx as a reverse proxy
Create a ngnix proxy as Dockerfile
Build the image for reverse proxy
Task 4 - Create and Run the containers for all the Images
Use docker run to create and run the image as container. Do this for all the services and reverse proxy.
Task 5 - Docker compose
Use docker-compose to deploy the completed application
Bonus: Use docker compose to build our images.

Solution
If you need help, you may refer to the solution available at /lesson-3-Container/solution/.