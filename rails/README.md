Edit [docker-compose.yml](docker-compose.yml) to configure the
services you want and their configuration.

To build the containers run:

```bash
docker-compose build
```

To run the containers run:

```bash
docker-compose up
```

When you modify the [Gemfile](app/Gemfile) run bundler as
you would normally do in any rails application:

```bash
docker-compose run web bundle install
```

All service data, including bundler's, are stored under `./app/tmp/`.

It goes without saying that, to run the application in a different version of ruby or rails you need to modify the [Dockerfile](app/docker/Dockerfile) and the [Gemfile](app/Gemfile).
