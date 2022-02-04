# Multiple containers - swarm

Test web app that returns the name of the host/pod/container servicing req

This folder contains the files to build a multiple containers web app using swarm

## How to run

1. Build an image

       docker image build -t elenavolkova/docker-learning:swarm .

2. Run container

       docker stack deploy -c docker-compose.yml counter

3. Open the web app

       http://localhost:5000/

4. View containers stack 

       docker stack ps counter

5. Remove containers stack

        docker stack rm counter