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

## Hosted Platform Notes

* Safari not supported, used Chrome

### Part 1:  MLRun Basics

Must do TWO THINGS before you run [tutorial](https://docs.mlrun.org/en/latest/tutorial/01-mlrun-basics.html) on hosted platform:

1. !/User/align_mlrun.sh
2. Restart Kernel







## Install Notes
### Getting started with official docs

* Locally use Docker Desktop as described in [Install MLRun on a Kubernetes Cluster](https://docs.mlrun.org/en/latest/install.html#install-mlrun-on-a-kubernetes-cluster)

* Follow steps described.


### Getting Started via manual install and Github README 

* Install (Make sure you have the latest `pip`).  Install on OS X will take several minutes and requires Rust and Cython.

* Create and source a python virtualenv:  `python3 -m venv ~/.mlrun-notes && source ~/.mlrun-notes/bin/activate`
`pip install --upgrade pip && pip install mlrun`


### Common Install Errors and Gotchas for Manual Install

### Operating Specific:
#### OS X 
 
 Can take 30+ minutes to install and contains many dependency errors.
 
  * install latest Python and Rust):  `brew install python` and `brew install rust`  
  * `ModuleNotFoundError: No module named 'Cython'`
  * `RuntimeError: cargo not found in PATH. Please install rust (https://www.rust-lang.org/tools/install) and try again`
  * `clang: error: the clang compiler does not support 'faltivec', please use -maltivec and include altivec.h explicitly`
  * `ERROR: Could not build wheels for maturin, which is required to install pyproject.toml-based projects`

#### Github Codespaces

* Install only takes a couple of minutes to install

### Tutorial Specific:

* [Automated Code Deployment and Containerization-Example](https://github.com/mlrun/mlrun#automated-code-deployment-and-containerization)

```
(.mlrun-notes) ➜  functions git:(main) ✗ mlrun build function.yaml

> 2021-11-26 11:39:57,419 [info] remote deployment started
> 2021-11-26 11:39:57,419 [error] database connection is not configured
> 2021-11-26 11:39:57,419 [info] building image (.mlrun/func-default-remote-git-test-latest)
deploy error, local docker registry is not defined, set DEFAULT_DOCKER_REGISTRY/SECRET env vars
```

* Replace README.md with [official docs link which is up to date and mentions Docker based workflows](https://docs.mlrun.org/en/latest/tutorial/01-mlrun-basics.html#introduction-to-mlrun)


## Potential Enhancements

* Hello World example in "one line"
* Target environment recommendation:  Github Codespaces, AWS Cloudshell, etc
* Hello World using a pre-built Docker pull command
* Separate demos with foolproof "hello world" commands for each architectural component
* More clear link to official docs

## References

* [mlrun](https://github.com/mlrun/mlrun) 
* [Watch on Pragmatic AI Labs](https://lnkd.in/ee9CXrsp)
* [Watch on O'Reilly Media](https://lnkd.in/eQ2YCjq)
