# Jenkins

* `docker build -t jenkins .`
* `docker run jenkins`

Ports

* 8080

# Amara Configuration
To create the Jenkins project for Amara, create a new job with the following:

* Source Code Management
  * Git: https://github.com/pculture/unisubs.git
* Poll SCM: `* * * * *`
* Add Build Step
  * Execute Shell: `/bin/test.sh <DOCKER_HOST_IP>`
