Apache felix
===================

> **IMPORTANT:** This is a beta version and is still in progress.

This image may be used to run a container with Apache felix.

### Usage

To run the container, the fastest command is:
```
docker run -it lucapalano/felix
```
To run and assign a name
```
docker run -it --name <name> lucapalano/felix
```
To make persistent your bundles installation, configuration, etc, you must add a data volume by usint the **-v** option as follow:
```
docker run -it --name <name> -v /home/felix lucapalano/felix
```
*/home/felix* is the path where felix is installed in the container and where your bundles configuration and installation will reside.

When starting the container, you must use the option **-i** in order to be sure that the felix gogo shell is available.


----------
*Apache Felix, Felix, Apache, the Apache feather logo, and the Apache Felix project logo are trademarks of The Apache Software Foundation. All other marks mentioned may be trademarks or registered trademarks of their respective owners.*