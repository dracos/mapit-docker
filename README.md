## Dockerized Mapit
### This is a work in progress and not yet ready to be used

###How to run this

You actually don't need this repository to try it out. The docker image built from this is
automatically available from the [Docker Hub](https://hub.docker.com/).

First, you'll need to install [Docker](https://docs.docker.com/) if you don't already have it.

Then,
```
docker pull openaustralia/mapit
docker run -p 8020:80 -i -t openaustralia/mapit
```

Point your web browser to [http://localhost:8020](http://localhost:8020) and you should see a
default install of Mapit.

All this without the hassle of having to configure a whole machine.

###What it does
* It will build a container that has everything needed to run Mapit.
* Runs the processes at startup managed by supervisord

###What it doesn't do
* Create a django admin user (TODO)
* Install an ssh server (TODO)
* Install data (TODO: An Australian mapit with data preloaded as a separate docker image)
* Setup logging for processes
