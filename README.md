## Heroku Cedar Stack images

This repository holds recipes for building the modified [Heroku Cedar stack images](https://devcenter.heroku.com/articles/cedar). This image have [libicu-dev](http://packages.ubuntu.com/trusty/libicu-dev) installed. The recipes are also rendered into Docker images that are [available on Docker Hub](https://registry.hub.docker.com/u/donnykurnia/heroku-cedar-libicu/). [Lists of packages installed on the current Cedar stacks](https://devcenter.heroku.com/articles/cedar-ubuntu-packages) are published on Heroku Dev Center.

This image can be used as replacement for the original cedar image in your Dockerfile. Replace `FROM heroku/cedar:14` with `FROM donnykurnia/heroku-cedar-libicu:14` and now you are using base image with libicu-dev already installed.
