# mlrun-notes
A repository for notes on [mlrun](https://github.com/mlrun/mlrun)

![mlrun-architecture](https://user-images.githubusercontent.com/58792/143601378-a3d957f9-b24e-4d7b-a990-3faf769b1e9f.png)

## What is it?

*  open-source MLOps framework
*  abstraction layer to a variety of technology stacks

## Architectural Components

* Feature and Artifact Store
* Elastic Serverless Runtimes:  Kubernetes/Nuclio/Dask/Spark/Horovod
* ML Pipeline Automation:  data prep/modeling/real-time pipelines/monitoring
* Central Management: UI/CLI/SDK

## Key Features

* Speed of deployment
* Elastic scaling of batch and real-time jobs
* Feature management system
* Runs anywhere

## Core Concepts

* Project
* Function
* Run
* Artifact
* Workflow
* UI

## Getting Started

* Install (Make sure you have the latest `pip`).  Install will take several minutes and requires Rust and Cython.

Create and source a python virtualenv:  `python3 -m venv ~/.mlrun-notes && source ~/.mlrun-notes/bin/activate`
`pip install --upgrade pip && pip install mlrun`


## Common Install Errors and Gotchas

* Operating Specific:
  * OS X (install latest Python):  `brew install python`   

* `ModuleNotFoundError: No module named 'Cython'`


## References

* [mlrun](https://github.com/mlrun/mlrun) 
