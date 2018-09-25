# Docker-SampleNodeApp
This is the repo for Simple Hello world web app running with docker.
Dockerfile is required to which Docker uses to build a docker image.
npm need to be installed on the machine.
To build an image from docker file, run following command where Dockerfile is situated:
docker build -t <docker-hub-username>/node-web-app .
"docker ps" command is used to see the running process in any container with their container-d
"docker images" command is used to see all created images
"sudo docker run <user_name>/node-web-app -d -p localPort:DockerexposedPort" to run the image. Ports need to be mapped. The -p flag redirects a public port to a private port inside the container. 
Running your image with -d runs the container in detached mode, leaving the container running in the background.

To test, run "docker ps"
Now you can call your app using curl 
$ curl -i localhost:localPort
