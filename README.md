[![CircleCI](https://circleci.com/gh/mehmetincefidan/Operationalize-a-Machine-Learning-Microservice-API/tree/master.svg?style=svg)](https://circleci.com/gh/mehmetincefidan/Operationalize-a-Machine-Learning-Microservice-API/tree/master)

# Project 4: Operationalize a Machine Learning Microservice API 

## Project Overview

In this project, I applied the skills I have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

The  project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:

* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

---

### Setup the Environment

* Create a virtualenv and activate it

```
python3 -m venv ~/.devops
source ~/.devops/bin/activate
```

* Run `make install` to install the necessary dependencies
```
make install
```

### Docker

* Docker installation
* Lints checks with hadolint and pylint
* Installation of Kubernetes and Minikube

### Kubernetes

* Configure Kubernetes to Run Locally
* Deploy with Kubernetes
* Savings Output logs in the file kubernetes_out.png

### CircleCI Integration

This repository has been verified with CircleCI

### Files
```
/.circleci : CircleCI configuration file
/model_data : Housing model data
/output_txt_files : Log of Output 
Dockerfile : Dockerfile for building the image 
Makefile : environment setup and lint tests
app.py : Python flask app that serves out predictions (inference) about housing prices through API calls
make_prediction.sh : Send a request to the Python flask app to get a prediction for localhost 
requirements.txt : packages dependencies 
run_docker.sh : shell script to get Docker running locally
run_kubernetes.sh : shell script to to run the app in kubernetes
upload_docker.sh : shell script to upload the image to docker
```
