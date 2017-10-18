# Docker_made_easy
 My experience of learning docker.
## Step by step guide
1. Download docker setup on your OS.

2. Setup you account on [dockerhub](https://hub.docker.com/) .

3. Pull your first image from dockerhub.
```
  $ docker run alpine
 ```
4. For checking the details of images 
```
  $ docker images
```
5. List of all the running containers
```
  $ docker ps -a
```
6. To stop alpine
```
  $ docker stop alpine
```
7. To create an container
```
  $ docker create alpine 
```
8. To remove a container
```
  $ docker kill alpine
```
9. To remove an image 
```
  $ docker rmi <image_name>
```
## To build your own image 

