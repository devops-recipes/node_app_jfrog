# Build and Push a Docker image for a Node JS application

[![Run Status](https://api.shippable.com/projects/5ac6a85f54f7fe070052d7ef/badge?branch=master)](https://app.shippable.com/github/devops-recipes/node_app_jfog) [![Coverage Badge](https://api.shippable.com/projects/5ac6a85f54f7fe070052d7ef/coverageBadge?branch=master)](https://app.shippable.com/github/devops-recipes/node_app_jfog)

![AyeAye](https://github.com/devops-recipes/push-docker-hub/blob/master/public/resources/images/captain.png)

A simple Node JS application with unit tests and coverage reports using mocha
and istanbul. It also does a docker build once CI posses and then pushes the image
to JFrog artifactory.

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](wwww.shippable.com)
* Create an [integration](http://docs.shippable.com/platform/integration/jfrog-artifactoryKey/#jfrog-artifactory-integration) on shippable to your docker hub
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `shipDH`
* Change the DOCKER_REPO and DOCKER_ACC to point to your repo and docker account
* You should be able to run a manual build or webhook build on commit
