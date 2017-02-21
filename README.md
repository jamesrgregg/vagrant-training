# Project Details

Date: 2017-02-20



## Project Setup
Vagrant up using Vagrantfile for 3 hosts
ssh to each of the hosts
 - acs will become the Ansible Control Server (ACS)
    - sudo apt-get update
    - sudo apt-get install ansible

 - docker
    - sudo apt-get update
    - sudo apt-get install docker.io
    - sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 36A1D7869245C8950F966E92D8576A8BA88D21E9
    - sudo sh -c "echo deb https://get.docker.com/ubuntu docker main\ > /etc/apt/sources.list.d/docker.list"
    - sudo apt-get update
    - sudo apt-get install lxc-docker

 - jira within Docker containers
    - sudo apt-get update
    - sudo apt-get install docker.io
    - sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 36A1D7869245C8950F966E92D8576A8BA88D21E9
    - sudo sh -c "echo deb https://get.docker.com/ubuntu docker main\ > /etc/apt/sources.list.d/docker.list"
    - sudo apt-get update
    - sudo apt-get install lxc-docker
    - sudo docker run --name jiradb-postgres -e POSTGRES_PASSWORD=strongpostgrespw -d postgres
    - sudo docker run --detach --publish 8080:8080 --link jiradb-postgres:postgres --name jira7 cptactionhank/atlassian-jira-software:latest

 ## Note: 
    - docker run --detach --publish 8080:8080 cptactionhank/atlassian-jira:latest
    

## References
* Docker install on ubuntu
    - http://buildvirtual.net/docker-installing-docker-on-ubuntu-trusty-14-04/
* Atlassian JIRA wrapped in a Docker image 
    - https://hub.docker.com/r/cptactionhank/atlassian-jira/
* JIRA Docker Quick Setup
    - https://www.becodemonkey.com/2016/02/15/jira-docker-quicksetup/
* Jira binaries
    - https://my.atlassian.com/product