# Docker Java 8 helloworld

Example [Docker](https://www.docker.com/) image that when echos "Hello world!" when run.

![terminal gif](https://raw.githubusercontent.com/stevenalexander/docker-java8-helloworld/master/terminal.gif "terminal gif")

Image has JRE rather than JDK to limit installed components. Tested on Mac using [Boot2Docker](http://boot2docker.io/) (v1.5.0).

Requires:
* [Docker](https://www.docker.com/)
* [Boot2Docker](http://boot2docker.io/)
* JDK (to compile java file locally)

To run:

```
# compile class
javac helloworld.java

# build image
docker build -t java8-helloworld .

# run image
docker run -it --rm --name my-running-app java8-helloworld
```
