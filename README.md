# Docker Tutorial

## Description

This github respository acts as a personal record of the [tutorial from Docker](https://docs.docker.com/get-started/02_our_app/). 

## Testing

The public docker repository can be found [here](https://hub.docker.com/r/geerma/getting-started). 

- Type ```docker pull geerma/getting-started```
- Then ```docker run -dp 3000:3000 geerma/getting/started:bindmount```
- Visit [http://localhost:3000](http://localhost:3000) (or whichever port you have set it to)

## Container Image

A Container Image is an immutable file that contains everything needed to create a virtual environment and run an application - such as the configuration settings for the container itself (eg. environment variables) as well all source code, libraries, dependencies. Since the settings of the container is specified, this allows developers to test applications in stable work environments.

- To create a Docker image, the developed should create a ```Dockerfile``` in  the application's directory
- An example of the command used to build and image is: ```docker build -t getting-started .```

## Docker Container

A Docker Container is a virtualized run-time environment that allows users to start and isolate applications using an *image*. 

- An example of the command used to run an application is: ```docker run -dp 3000:3000 getting-started```



