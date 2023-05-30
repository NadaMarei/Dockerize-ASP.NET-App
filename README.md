# Dockerize-ASP.NET-App

## Dockerizing an ASP.NET App
This repository contains an example of how to Dockerize an ASP.NET app. Creating a Docker image that contains all the necessary components for the app to run, including the .NET Core runtime, any dependencies, and the app code itself. This image can then be used to spin up one or more Docker containers, each of which runs an instance of the app. The steps below will guide you through the process of building and running the Docker container.

## Prerequisites
Before you begin, make sure you have the following installed:
- Docker
- .NET Core SDK

## Building the Docker Image
- Clone this repository to your local machine.
- Open a terminal or command prompt and navigate to the root directory of the cloned repository.
- Build the Docker image by running the following command:

`docker build -t aspnet-app . `
  This will create a Docker image with the tag aspnet-app.

## Running the Docker Container
Once the Docker image is built, run the following command to start the container:

`docker run -p 8080:80 aspnet-app`
 This will start the container and map port `8080` on your local machine to port `80` in the container.

Open a web browser and navigate to `http://localhost:8080`. You should see the `ASP.NET app` running.

## Customizing the ASP.NET App
If you want to customize the ASP.NET app, you can modify the code in the src directory and then rebuild the Docker image.
