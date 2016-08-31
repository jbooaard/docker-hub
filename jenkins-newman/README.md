Jenkins + Newman
===================
This include the latest jenkins server and newman which can be used in order to run your postman collections.

[![Jenkins](https://raw.githubusercontent.com/docker-library/docs/3ab4dafb41dd0e959ff9322b3c50af2519af6d85/jenkins/logo.png)](https://jenkins.io/)

[![newman](https://www.getpostman.com/img/v2/apps/newman.png?5a73d3948bd3148b754c1ac5e0c24fcd)](https://www.npmjs.com/package/newman)


### Usage
The fastest command to run the container:
```
docker run -p 8080:8080 -p 50000:50000 lucapalano/jenkins+newman
```
The fastest command to run and assign a name:
```
docker run -p 8080:8080 -p 50000:50000 --name <name> lucapalano/jenkins+newman
```
All jenkins data resides in */var/jenkins_home* . You may want to make that volume persisten with the following command:
```
docker run -p 8080:8080 -p 50000:50000 -v /var/jenkins_home lucapalano/jenkins+newman
```
When starting the container, you may add the **-i** option in order to be sure that jenkins log will be printed on your bash stdout:
```
docker start -i <containerid>
```
Further informations about container data backup, jenkins and jvm configuration, etc can be founded to [the official docker hub jenkins page](https://hub.docker.com/_/jenkins/) (highly recommended).

### Author

Luca Palano - contact@lpzone.it

### Contribute

Contributions, questions, and comments are all welcomed! Fork and create a pull request on github: https://github.com/lucapalano/docker-hub/tree/master/jenkins-newman

----------
*Postman, Newman, Jenkins, the newman and jenkins logos are trademarks of their respective owners.*

https://www.getpostman.com/
https://jenkins.io
