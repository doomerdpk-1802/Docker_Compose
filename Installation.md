# Manual Installation:

- Install NodeJS and Mongo DB.
- Clone the repository using command "git clone https://github.com/doomerdpk-1802/Docker_Compose.git"
- Copy environment variables file using command "cp .env.example .env" and Replace the DATABASE_URL by an actual URL.
- Run "npm install" to install all the dependencies.
- Run "npm run start" to start the application.


# Installation using Docker:

  - Install Docker.
  - Clone the repository using command "git clone https://github.com/doomerdpk-1802/Docker_Compose.git"
  - Build the backend image using the command "docker build -t image_name ."
  - create a network using comamnd "docker network create test_network"
  - start mongdb locally using the command "docker --name mongoDatabase --network test_network -d -p    
    27017:27017 mongo"
  - start the backend container using the command "docker --network test_network -e 
    mongodb://mongoDatabase:27017/my_db -d -p 3000:3000 image_name
  - Run command "docker ps" to see the status of both the conatiners.
  - Run command "docker logs container_id" to debug any errors.