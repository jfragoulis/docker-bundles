The repository contains a collection of application templates ready for use.

To start, clone the repo in a directory and copy the template files for the stack of your choice to a another folder.

To start with a vanilla rails application:

```bash
cd ~/apps
git clone git@github.com:jfragoulis/docker-bundles.git
cp -r docker-bundles/rails blog
cd blog
docker-compose build
docker-compose run web bundle install
docker-compose run
```

To setup the database, open another shell and run:

```bash
docker-compose run web bin/setup
```
