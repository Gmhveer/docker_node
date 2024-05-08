//This repository is Created for creating dockerization container with node backend server.

// Step clone docker_node

//On local setup 
    cmd: npm install
    cmd: npm start


// Run server using docker

    // Note: First You should have install docker app and run docker service on your local system

    info cmd: (check for list of docker images)
        - docker images 

    Build docker container:
        - docker build -t < container_name > .
    
    Run docker image container:
        - docker run -it -p 3000:3000 < container_name >

    Check Process of docker:(check running images || check in docker app)
        - docker ps