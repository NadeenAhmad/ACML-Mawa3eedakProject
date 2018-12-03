# Mawa3eedak :
* This is a simple todo list to help students organize and remember their tasks like quizzes , assignments , deadlines , projects and presentations

# Aim of project :
  - This project is a some sort of practice on the 12 factor app concept 
  - Our project complies by the following factors:
  - 0. README : In this repository you can see this written which clarifies how to use our project and modify it locally 
  - 1. I Codebase : Our private git repository was constantly updated with any code contribution to the project
  - 2. II Dependencies :
  - A dependency declaration manifest declares all dependencies of an app.In node js it is npm
  - A dependancy isolation tool is basically tool that ensures that no implicit dependencies “leak in” from the surrounding system , to avoid conlicts between version in the future . In node js it is npm.
  - 3. III Config : A separate Config file should be created when running the project to avoid hard-coding it you can find below in the READ.md how to create it & its content
  - 4. V Build, Run, Release : Our project contains a Dockerfile run off the application 
    Explaining the Dockerfile content: 
                     ![alt text](https://i.ibb.co/0ch8fDN/Slide1.jpg)
  - 5. IV Backing Services : 2 backing services are used 
    1 - Mongodb
    2 - JSON API
  - You can find in our project's directory a docker-compose.yml file that is used to bring up our app along with the backing services stated above docker-compose.yml content explained :
               ![alt text](https://i.ibb.co/XsFwRr4/Slide2.jpg)
                
# Prerequisites :
  - In order to run this project you only need Docker installed !!
  - You can find below some links that helps in the installation process: 
  - Linux Ubuntu 16.04: "https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-16-04"
  - Windows 10 Pro : "https://docs.docker.com/docker-for-windows/install/"
  - Mac : "https://docs.docker.com/docker-for-mac/" 
# Built with :
* Mean stack :
    - Mongodb
    - Express
    - Node js
# Backing Services used :
  - Mongodb
  - JSON API (containing usernames & passwords) :
           "https://api.myjson.com/bins/ujpdu" 
# How to use the project :
## Create a config file 
   - In the directory of your project create a saperate config file 
   - Inside it create a js file with the name "database"
   - export the following url in it : 'mongodb://mongo:27017/docker-node-mongo' 
              - if you wish to change the container name change "docker-node-mongo" to your new container name in the database.js and Dockerfile
## Run in Docker
   - docker-compose up
## Tear down
   - docker-compose down
## To re-build
   - docker-compose build

# Authors :
* Nadeen Ahmad 37-4023 
* Radwa Elshenawy 37-5390
* Mayar Alfares 37-2915
