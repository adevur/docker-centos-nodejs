# centos-nodejs
This image provides a minimal CentOS 7 image with Node.js and NPM installed.

### Tags
This image has two tags: `latest` and `lts`.

`centos-nodejs:latest`: based on current latest stable release of Node.js (11.x.x).

`centos-nodejs:lts`: based on current LTS release of Node.js (10.x.x).

### Building
To build `latest` tag:
```sh
docker build --tag=centos-nodejs:latest ./latest
```
To build `lts` tag:
```sh
docker build --tag=centos-nodejs:lts ./lts
```

### Usage
You can use this image as a base for other Docker images, by using `FROM: adevur/centos-nodejs:latest` in your Dockerfile.

Otherwise, you can also use this image as stand-alone. For example, if you run:
```sh
docker run --rm --name nodejs -it adevur/centos-nodejs:lts /bin/bash
```
You'll have a bash terminal opened in a container with CentOS 7, Node.js 10.x.x LTS and latest NPM version.

### Additional info
Node.js and NPM have been installed using the procedure described at: [NodeSource Node.js Binary Distributions](https://github.com/nodesource/distributions#rpm)
