# Overview
This repository implements the CI/CD pipeline for Python Flask Machine learning app using Microsoft Azure. 

## Project Plan
* [Trello](https://trello.com/b/C3ceeWmW/flask-ml-task)
* [Project Planning](https://docs.google.com/spreadsheets/d/1dxMQlkFInCwCUSMQBhnbmbo_12ffJuVlZAwjiTnfZjo/edit?usp=sharing)


## CI/CD Architectural
The flow diagram below depicts the high level of the architecture:
![Flow Diagram](./screen_shots/diagram.png)


The architectural Diagram can be divided into two parts as follow:

### Azure CI
The diagram below depicts the architecture of the Continuous Integration
![CI Diagram](./screen_shots/CI.png)

### Azure CD
The diagram below depicts the architecture of the Continuous Delivery
![CD Diagram](./screen_shots/CD.png)


## Instructions

<TODO:  Instructions for running the Python project.  How could a user with no context run this project without asking you for any help.  Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

### Project cloned into Azure Cloud Shell
Open the Azure Cloud Shell and clone the Github repository with the following command:
```
git clone GITHUB_URL_REPO
```
Replace the GITHUB_URL_REPO with the URL that stores the source code.

You can navigate to the folder after it has cloned the repository.

Example:
![Azure Shell](./screen_shots/01_AzureShell.png)

### Creating the Virtual Environment
On Azure shell, enter the following command to create virtual environment:
```
python3 -m venv ~/.my-repo
```

The <i>my-repo</i> is the name used for this project. You can use any name as you wish.

Once the virtual environment was created, enter the following command to activate the environment:
```
source ~/.my-repo/bin/activate
```
Example:
![Virtual Environment](./screen_shots/virtual_env.png)


### Install the dependencies via Makefile
Once you have the virtual environment installed, you can run the Makefile via:

```
make all
```

The command will install the dependencies and run the test script.

Output:
![Make Output](./screen_shots/02_Makefile_1.png)

![Make Output](./screen_shots/02_Makefile_2.png)


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


