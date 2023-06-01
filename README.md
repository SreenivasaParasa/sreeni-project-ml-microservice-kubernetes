[![CircleCI](https://dl.circleci.com/status-badge/img/gh/SreenivasaParasa/sreeni-project-ml-microservice-kubernetes/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/SreenivasaParasa/sreeni-project-ml-microservice-kubernetes/tree/main)

## Project Overview

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

Your project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

./run_docker.sh
 ./make_prediction.sh
./upload_docker.sh    
he push refers to repository [docker.io/sreenivasaparasa/api]
1d5b479efc25: Pushed 
a251694f09f2: Pushed 
650104debdce: Pushed 
42855dae5730: Mounted from library/python 
0e0c3e2a9021: Mounted from library/python 
e1bb4ba2013a: Mounted from library/python 
3284da728da0: Mounted from library/python 
a8e0bda64b48: Mounted from library/python 
54060bf84ed3: Mounted from library/python 
d1b4bcba0655: Mounted from library/python 
1c6f4c23073b: Mounted from library/python 
ef9ee2bbae58: Mounted from library/python 
latest: digest: sha256:df144ca4e6617a98678f8dd16114cb1a3f1ac29d1e9e76c9ae2eee22e573a54f size: 2845
(.devops) anirudhsriram@anirudhs-MacBook-Air project-ml-microservice-kubernetes % ./upload_docker.sh
Docker ID and Image: sreenivasaparasa/api
Password: 
Login Succeeded

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

1165  minikube start --driver=docker\n
 1166  kubectl config view
 1167  ./run_kubernetes.sh
 1168  kubectl config view
 1169  kubectl get pd
 1170  kubectl get pod
 1171  kubectl get pod
 1172  ./run_kuberenets.sh
 1173  lsw
 1174  ls -ltr
 1175  ./run_kubernetes.sh
 1176  minikube stop
 1177  git add .
 1178  git commit -m "check all files"
 1179  git push
