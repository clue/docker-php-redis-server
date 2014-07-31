# docker-php-redis-server

The [php-redis-server](https://github.com/clue/php-redis-server) is a pure PHP re-implementation
of the [redis](http://redis.io/) key-value store.
This is a [docker](https://www.docker.io) image that eases setup.
So now you can easily test-drive the implementation by replacing your normal redis container with this one.

## About php-redis-server

> *From [the official readme](https://github.com/clue/php-redis-server#readme):*

A redis server implementation in pure PHP. Not for the faint-hearted.

Why would I use this project if I already have the official redis server installed? Simply put, you wouldn't. Ever.

## Usage

This docker image is available as a [trusted build on the docker index](https://index.docker.io/u/clue/php-redis-server/),
so there's no setup required.
Using this image for the first time will start a download.
Further runs will be immediate, as the image will be cached locally.

The recommended way to run this container looks like this:

```bash
$ docker run -d --name redis clue/php-redis-server
```

This is a rather common setup following docker's conventions:

* `-d` will run a detached session running in the background
* `--name` will assign the given name to the running container instance
* `clue/php-redis-server` the name of this docker image
