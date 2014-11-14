

# Intro


# About me

* CTO O'Reilly Media
* A bit about O'Reilly

# About this talk

* Grew out of a conversation with Laurent Gautier about our "Just Enough Math" tutorial we gave
* Packaged a math tutorial written in IPython Notebook as a Docker container for a conference


Lessons learned about creating repeatable workflows for using IPython Notebooks and Docker

# Overview

* Quick intro to IPython Notebook
* IPython Notebook ecosystem on GitHub
* Using Docker notebooks and dependencies to make shareable environments


# IPython Notebooks -- a platform for repeatable computation

# Show a bit about the gui


# show a bit about the ipynb format


# Collaborate using git and GitHub

* Because it's text, you can collaborate w/colleagues on GitHub

* Easy way to share work with colleagues

* flow workflow (branch -- commit -- merge), although it can be painful with JSON



# Key Workflow issue we ran into on Just Enough Math

* Setting up notebook server itself
  * conda package can help
* Project specific dependencies
  * Numerical computing libraries are hard to install
  * Platform specific package managers -- apt, yum, brew, macports, whatever windows uses
  * Language specific package manages -- pip, setup\_tools_, virtualenv, npm, gem, bundler, and on and on

# Docker -- a way to snapshot and share the computing environment


# Install Docker

this can be the hardest part

# Add a Dockerfile

* FROM ipython/scipystack

* Add dependencies and other requirements in this file

* Docker build to create an image


# Add a fig.yml

* Expose port
* start the notebook server
* Use a Volume to link container to host so that when you press "Save" it saves on the host, rather than the container

  * Available only on mac
  



