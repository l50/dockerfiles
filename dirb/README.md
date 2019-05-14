# dirb
[![Build Status](https://img.shields.io/docker/cloud/build/l505/dirb.svg)](https://cloud.docker.com/repository/docker/l505/dirb/builds)
[![Docker Pulls](https://img.shields.io/docker/pulls/l505/dirb.svg)](https://hub.docker.com/r/l505/dirb)
[![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/l50/dockerfiles/blob/master/LICENSE)

A dockerized version of [dirb](http://dirb.sourceforge.net/).

## Setup
Pull down the image:
`docker pull l50/dirb`

## Usage
Get help menu options: `docker run --rm -v ${PWD}:/dirb l50/dirb`

To run against a site and send the output to a dirb directory in your current working directory:
`docker run --rm -v ${PWD}/dirb:/dirb l50/dirb https://somesite.com -o /dirb/somesite`

