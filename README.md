## Table of contents
* [General info](#general-info)
* [Architecture](#architecture)
* [Setup](#setup)

## General info
This repository is made by data scientists for data scientits. It has the aim to reduce the time searching for installers and libraries when starting a new project. It also considers the necessity to orchestrate the ML pipelines [Airflow](https://github.com/apache/airflow) and to track and register the models [MLFlow](https://github.com/mlflow/mlflow).
	
## Architecture

![alt text](https://github.com/JCirera/MLproject-skeleton/blob/main/Architecture.jpg?raw=true)

NOTE: 
* The python and airflow container is based on [puckel](https://github.com/puckel/docker-airflow) with some modifications due to specific requirements of snap7 library.
* There is a fifth container, hidden in the architecture diagram, to wait for dependencies. It is courtesy of [dadarek](https://github.com/dadarek/docker-wait-for-dependencies)
	
## Setup
To run this project, clone the repo and run the next command in the project folder:

```
docker-compose -f docker-compose-skeleton.yml up
```
NOTE: it is necessary to have [Docker](https://github.com/docker) and [Docker Compose](https://github.com/docker/compose) installed in your host machine.
