# node-docker

A barebones Node.js app using [Express 4](http://expressjs.com/).

# Steps
Follow the Below steps
# Take a git clone of this repo git clone 
https://github.com/Krishank/node-docker.git
cd node-docker

# Now Create your own image by running comand: 
docker build -t <nameOfYoutImage>:<tag> . 

You can run like this: docker build -t node-docker:v1 .

# Check the image is created or not: 
docker images or docker images | grep <nameOfYoutImage>:<tag>
You can run like this: docker images | grep node-docker:v1

# Run your Docker image
docker run  -it -p <portToExpose>:<portInAppIsRunningInsideContainer> <nameOfYoutImage>:<tag>
You can run like this: docker run -d -p 3001:3001 node-docker:v1

# check all docker container running
docker ps

# Delete a Docker images
docker image rm -f <nameOfYoutImage>:<tag>
docker image rm -f node-js-sample:v1

# For more comands 
https://docs.docker.com/engine/reference/commandline/docker/
