Apache felix
===================

This image may be used to run a container with Apache felix.

### Available versions
- 5.6.1 (latest)
- 5.4.0

### How to use this image

The fastest command to run the container:
```
docker run -it lucapalano/felix:latest
```

The fastest command to run and assign a name:
```
docker run -it --name <name> lucapalano/felix
```

This will make persistent your bundles installation, configuration, etc... (everything under /home/felix):
```
docker run -it --name <name> -v /home/felix lucapalano/felix
```
*/home/felix* is the path where felix is installed in the container and where your bundles configuration and installation will reside.

When starting the container, you must use the option -i in order to be sure that the felix gogo shell is available, as follow:
```
docker start -i <containerid>
```

### Author
Luca Palano - contact@lpzone.it

----------
*Apache Felix, Felix, Apache, the Apache feather logo, and the Apache Felix project logo are trademarks of The Apache Software Foundation. All other marks mentioned may be trademarks or registered trademarks of their respective owners.*

http://www.apache.org
http://felix.apache.org
