# one container - dockerfile

Test web app that returns the name of the host/pod/container servicing req

This folder contains the files to build a single container web app using dockerfile

## How to run

1. Build an image

       docker image build -t elenavolkova/docker-learning:one-container .

2. Run container

       docker container run -d --name test-container-1 -p 8000:8080 elenavolkova/docker-learning:one-container

3. Open the web app

       http://localhost:8000/

4. Stop/start container

       docker container stop test-container-1
       docker container start test-container-1

5. Remove container 
   
       docker container rm test-container-1