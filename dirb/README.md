# dirb

A dockerised version of [dirb](http://dirb.sourceforge.net/)

## Setup
Pull down the image:
`docker pull l50/dirb`

## Usage
Get help menu options:
`docker run --rm -v ${PWD}:/dirb l50/dirb`

To run against a site and send the output to a dirb directory in your current working directory:
`docker run --rm -v ${PWD}/dirb:/dirb l50/dirb https://somesite.com -o /dirb/somesite`
