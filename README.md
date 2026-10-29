# ci-cd-final-project

## Project Name
ci-cd-final-project

## Overview
A Python sample application demonstrating continuous integration and continuous deployment (CI/CD) using GitHub Actions, Tekton tasks, and OpenShift Pipelines.

## Technologies
- Python
- GitHub Actions
- flake8
- nose
- Tekton Pipelines
- OpenShift

## Project Files
- `app.py` — Sample application functions
- `tests/test_app.py` — Unit tests
- `.github/workflows/workflow.yml` — GitHub Actions linting and unit-testing workflow
- `.tekton/tasks.yml` — Tekton cleanup and nose unit-testing tasks
- `.tekton/pipeline.yml` — OpenShift Pipeline configuration
- `.tekton/pvc.yml` — PersistentVolumeClaim configuration

## Run Locally

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Run linting:

```bash
flake8 app.py tests
```

Run unit tests:

```bash
nosetests -v
```

## GitHub Actions
The GitHub Actions workflow runs on pushes and pull requests to the `main` branch. Check the Actions tab in this repository to review the actual workflow execution results.

## OpenShift and Tekton
The `.tekton/` directory contains the Tekton task and pipeline manifests used for the CI/CD project. Apply these resources only in the OpenShift project provided by the course lab and follow the lab instructions.

## Project Goal
The goal of this project is to demonstrate automated code linting, unit testing, container image building, and application deployment through a CI/CD pipeline.

## Verification
Use the actual GitHub Actions results and OpenShift pipeline runs to verify successful execution. Screenshots and logs submitted for the course should come from the actual project environment.