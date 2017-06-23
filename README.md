# docker-moodle

[![GitHub release](https://img.shields.io/github/release/radioberry/docker-moodle.svg)]()
[![Build Status](https://travis-ci.org/radioberry/docker-moodle.svg?branch=master)](https://travis-ci.org/radioberry/docker-moodle)

## Description

Moodle - the world's open source learning platform

docker:
 - https-portal
 - moodle
 - mysql 

## Demo


## Usage

```
docker-compose up -d
```
You can visit the following URL in a browser to get started:

https://moodle.example.com


## Install

```
git clone https://github.com/radioberry/docker-moodle.git
cd docker-moodle
docker-compose build
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
