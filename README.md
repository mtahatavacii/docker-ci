# Hello World Flask Application

This project contains a simple Hello World Flask application implemented in Python. The application provides an endpoint that returns a greeting message.

## Prerequisites

Before running the application, ensure that you have the following dependencies installed:

- Python 3.x
- Docker 

## Local Development

To build the Docker container image and run the application locally, follow these steps:

1. Clone the repository.
2. Build a Docker container image and run the application inside a container:
   docker build -t your-image-name .
3. Run the Docker container using the built image:
  docker run -d -p 5000:5000 your-image-name

The application will be accessible at http://localhost:5000.

## Continuous Integration
This project is set up with continuous integration using GitHub Workflows. The workflow configuration can be found in the .github/workflows directory.

The workflow is triggered on push events to the main branch and also runs periodically on Saturdays at 7 PM. It builds the container image and pushes it to the Docker Hub registry with the latest tag.

You can find the built container image on Docker Hub: your-dockerhub-repo/your-image-name

