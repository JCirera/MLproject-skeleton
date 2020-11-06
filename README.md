## Table of contents
* [General info](#general-info)
* [Architecture](#architecture)
* [Setup](#setup)
* [Discussion and conclusions](#discussion-and-conclusions)

## General info
This repository is made by data scientists for data scientits. It has the aim to reduce the time searching for installers and libraries when starting a new project. It also considers the necessity to orchestrate the ML pipelines with [Airflow](https://github.com/apache/airflow) and to track and register the models with [MLFlow](https://github.com/mlflow/mlflow).
	
## Architecture

![alt text](https://github.com/JCirera/MLproject-skeleton/blob/main/Architecture.jpg?raw=true)

NOTE: 
* The python and airflow container is based on [puckel](https://github.com/puckel/docker-airflow) with some modifications due to specific requirements of snap7 library.
* There is a fifth container, hidden in the architecture diagram, to wait for dependencies. It is courtesy of [dadarek](https://github.com/dadarek/docker-wait-for-dependencies).
	
## Setup
To run this project, clone the repo and run the next command in the project folder:

```
docker-compose -f docker-compose-skeleton.yml up
```
NOTE: it is necessary to have [Docker](https://github.com/docker) and [Docker Compose](https://github.com/docker/compose) installed in your host machine.

## Discussion and conclusions
Any insight or suggestion in order to correct bugs or improve the architecture is welcome. The goal is to facilitate the job to the data scientits at the beginning of the projects.
