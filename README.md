# zeitgeist/docker-sslscan

[sslscan](https://github.com/rbsec/sslscan) (fork) in a Docker container.

## Requirements

* [Docker](https://www.docker.com/) 1.5+ (previous versions may work fine, but I haven't tried)

## Installation

Get the [trusted build on the docker hub](https://registry.hub.docker.com/u/zeitgeist/docker-sslscan/):

```bash
$ docker pull zeitgeist/docker-sslscan
```

or download and compile the source yourself from Github:

```bash
$ git clone https://github.com/alexzeitgeist/docker-sslscan.git
$ cd docker-sslscan
$ docker build -t zeitgeist/docker-sslscan .
```

## Usage

This is a fork of ioerror's version of sslscan. It tests SSL/TLS enabled services to discover supported cipher suites.

Example usage:

```bash
$ docker run --rm zeitgeist/docker-sslscan www.zeitgeist.se
```
