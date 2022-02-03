# Overview
This repository implements the CI/CD pipeline for Python Flask Machine learning app using Microsoft Azure. 

## Project Plan
* [Trello](https://trello.com/b/C3ceeWmW/flask-ml-task)
* [Project Planning](https://docs.google.com/spreadsheets/d/1dxMQlkFInCwCUSMQBhnbmbo_12ffJuVlZAwjiTnfZjo/edit?usp=sharing)


## CI/CD Architectural
The architectural Diagram can be divided into two parts as follow:

### Azure CI
The diagram below depicts the architecture of the Continuous Integration
![CI Diagram](./screen_shots/CI.png)

### Azure CD
The diagram below depicts the architecture of the Continuous Delivery
![CD Diagram](./screen_shots/CD.png)


## Instructions

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

* Project running on Azure App Service

* Project cloned into Azure Cloud Shell

* Passing tests that are displayed after running the `make all` command from the `Makefile`

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

* Running Azure App Service from Azure Pipelines automatic deployment

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```

* Output of streamed log files from deployed application

> 

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>


