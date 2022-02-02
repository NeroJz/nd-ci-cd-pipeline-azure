# nd-ci-cd-pipeline-azure
Deploying Flask Machine Learning Web App using CI/CD in Azure


## Instructions

### Create a virtual environment
In the azure shell run the following command:
```
python3 -m venv ~/.my-repo
```

To activate the virtual environment, run:
```
source ~/.my-repo/bin/activate
```

### Configure Github Actions
Navigate to the github repository.

Go to Actions > Set up the work yourself

Replace the main.yml with the following code

```
# This is a basic workflow to help you get started with Actions

name: Python application test with Github Actions

on:
  push:
    branches: [ master ]
  pull_request:
    branches: [ master ]

  # Allows you to run this workflow manually from the Actions tab
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v2
    - name: Set up Python 3.6
      uses: actions/setup-python@v1
      with:
        python-version: 3.6
    - name: Install dependencies
      run: |
        make install
    - name: Lint with pylint
      run: |
        make lint
    - name: Test with pytest
      run: |
        make test
```

Save and run main.yml. The output should be illustrated as follow:

![Github Actions](./screen_shots/03_GithubActions.png)