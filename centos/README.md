My centos
===================

This is an image built from centos:latest with some useful tools (\*):

* git
* golang
* man
* accountservice
* vim
* wget
* openjdk 1.8
* nodejs 4.x

(\*) _Where version is not specified, the default vendor version will be installed_

### How to use this image

The fastest command to run the container:
```
docker run -it lucapalano/centos
```

The fastest command to run and assign a name:
```
docker run -it --name <name> lucapalano/centos
```
### NOTE
This images may be subjected to changes according to my own requirements. I hope that someone will find this useful. Any suggestion is always welcome.

### Author
Luca Palano - contact@lpzone.it

----------
http://www.centos.org/
