# docker-moodle

[![GitHub release](https://img.shields.io/github/release/radioberry/docker-moodle.svg)]()
[![Build Status](https://travis-ci.org/radioberry/docker-moodle.svg?branch=master)](https://travis-ci.org/radioberry/docker-moodle)

## Description

Moodle - the world's open source learning platform

Configuration of docker-compose:
 - https-portal
 - moodle
 - mysql 

## Demo


## Usage

### FULL
```
docker-compose up -d
```
You can visit the following URL in a browser to get started:

https://moodle.example.com

### Combined with other domains
```
docker-compose up -d moodle moodle_db
```
or
Comment out docker-compose.yml's https-portal.
```
#   https-portal:
#     image: steveltn/https-portal:latest
#     ports:
#       - '80:80'
#       - '443:443'
#     links:
#       - moodle
#       - moodle_db
# restart: always
```

AWS Route53>Cloudfront>EC2(docker):

https://{AWSRoute53}

## Install

### FULL
```
git clone https://github.com/radioberry/docker-moodle.git
cd docker-moodle
docker-compose build
```

### Combined with other domains
```
git clone https://github.com/radioberry/docker-moodle.git
cd docker-moodle
docker-compose build moodle moodle_db
```


## Deploy

```
cd docker-moodle
emacs Dockerfile
~
docker-compose stop
docker-compose up -d
```

## Licence

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](LICENSE)

## Author

[tcnksm](https://github.com/tcnksm)
