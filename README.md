# DockerDemo

# ToDo App with Angular and Docker

## Description
This project is a simple ToDo application built with Angular. It allows users to add, edit, and delete TODO Tasks. The application is containerized using Docker.

## Application Functionality
- Add a Todo Task 
- Edit a task
- Delete a task

## Steps to Build and Run the Application

### Prerequisites
- homeBrew : https://brew.sh/
- Docker Desktop : https://www.docker.com/products/docker-desktop/
### Install Node
homebrew intsall node
verify  intsallation with - node --version
### Install Angular CLI
npm intsall angular/cli@12
verify  intsallation with : ng --version 
### Building the Angular Application and Dockerfile
1. Create Dockerfile inside your angular project root directory
2. Build Your Angular Project with following command: ng build --prod
3. now run Docker Build: docker build -t todo-app .
4. now run the docker container image and specify the port number :docker run -d -p 80:80 --name todo-app todo-app
### RUN / Verify
1. docker ps : to check running image
2. hit following url in browser: localhost
