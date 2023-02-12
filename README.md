[![CircleCI](https://dl.circleci.com/status-badge/img/gh/ohansck/Udacity-DevOps-Project4/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/ohansck/Udacity-DevOps-Project4/tree/main)

## Project Overview

## Housing Price Prediction API

This project operationalizes a machine learning API as a microservice that predicts housing prices in Boston. The API uses a pre-trained scikit-learn model to take into account various factors such as number of rooms, highway access, teacher-to-pupil ratios, and more. The project is flexible and can be adapted to any pre-trained machine learning model.

## Completed Tasks
- Code testing using linting
- Creation of a Docker container for the application
- Deployment of the container and demonstration of predictions
- Enhancement of log statements in the source code
- Configuration of a Kubernetes cluster
- Deployment of the container on the cluster and demonstration of predictions
- Upload of a GitHub repository with CircleCI integration to ensure code testing

## Repository Structure
- `.circleci`: for the CircleCI build server
- `model_data`: folder containing the pretrained scikit-learn model and housing CSV files
- `output_txt_files`: folder with sample output logs from running `run_docker.sh` and `run_kubernetes.sh` scripts
- `app.py`: the Flask application
- `Dockerfile`: instructions for containerizing the application
- `Makefile`: instructions for setting up the environment and lint tests
- `requirements.txt`: list of required dependencies
- `run_docker.sh`: script to build the Docker image and run the application in a Docker container
- `upload_docker.sh`: script to upload the built Docker image to Docker Hub
- `run_kubernetes.sh`: script to run the application in a Kubernetes cluster
- `make_prediction.sh`: script to make predictions using the Docker container and Kubernetes cluster
- `README.md`: the README file

## Instructions
1. Set up a virtual environment and activate it
2. Run `make install` to install the required dependencies
3. To run the application:
    - Standalone: `python app.py`
    - Docker: `./run_docker.sh`
    - Kubernetes: `./run_kubernetes.sh`

## Kubernetes Steps
1. Set up and configure Docker on your local machine
2. Set up and configure Kubernetes on your local machine
3. Create a Flask application in a container
4. Run the application using `kubectl`.

