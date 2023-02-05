## MA Online YouTube Video Downloader - Docker Image

## Overview
Do you want to create and run Docker Image?

Docker is an open-source platform for automating the deployment, scaling, and management of applications in containers. 
It provides a way to package and distribute software applications in a consistent and repeatable way, making it easier to manage dependencies and ensure that applications run the same way on different systems.

Docker uses containers, which are lightweight, stand-alone, and portable execution environments that can run software without affecting the underlying system. 
Containers allow developers to isolate their applications and dependencies from the host system, making it easier to manage the environment and ensuring compatibility between systems.

## Tools Used

- Docker Desktop
- VS Code


## How to Download

Download this project from here [Download MA Online YouTube Video Downloader Docker]
https://github.com/ma-muhammadali/pse_MAOnlineYouTubeVideoDownloader_Docker.git


## Requirements

## How to Create Docker Image

- Go to Docker Hub website and create your account (If not already created) 
	https://hub.docker.com/

- After creating account on Docker Hub, please download and install Docker Desktop software on your machine. 
	https://www.docker.com/products/docker-desktop/

- After installing Docker Desktop software, please run it and login into Docker Desktop using your account credentials created on Docker Hub.

- Download and Install Visual Studio Code (Windows Version) software from below URL. 
	https://code.visualstudio.com/download

- Download MAOnlineYouTubeVideoDownloader_Docker folder from GitHub repository and place it in VS Code workspace.
	
	https://github.com/ma-muhammadali/pse_MAOnlineYouTubeVideoDownloader_Docker.git

- Open MAOnlineYouTubeVideoDownloader_Docker in VS Code

- After selecting the Terminal as Bash, check the version of docker by running below command. $ docker -v

- Now we will create Docker Image by running below command.
	
	docker build -t muhammadaliofc1/maonlinevideodownloader:1.0.2.RELEASE .
	
	In this command, we will build a Docker image
	
	▪ muhammadaliofc1/maonlinevideodownloader is the name of the image
	▪ 1.0.2.RELEASE is the release number of this image

- Run below command and start the Container
	$ docker container run -d -p 3000:3000 muhammadaliofc1/maonlinevideodownloader:1.0.2.RELEASE
	
	▪ Here we are binding the host port with container port. Since we have exposed Port:3000 so we need to mention same in above command

- Check the status of Container by running below command
	$ docker container ls


## Usage

* After running Docker Image Container python terminal/ Docker Desktop and then goto http://localhost:3000/
* Paste a youtube video url and click Start
* Click Download Video, Download will start automatically
