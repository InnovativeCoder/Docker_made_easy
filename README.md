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

Make a dockerfile in your repository for which you want to make the image.
Open the docker file and write following into it :
```
FROM python:3.6

EXPOSE 8000

#install dependencies
COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt

#Run the code

CMD ["python3 <filename>"]
```
*instead of filename write the name of file you want to compile*
***above code can be edited on the basis of the language chosen***

