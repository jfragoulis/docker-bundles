# Managing submodules

[Documentation](https://git-scm.com/book/en/v2/Git-Tools-Submodules)

To checkout with the project templates:

```bash
git clone --recurse-submodules git@github.com:jfragoulis/docker-bundles.git
```

If you have already checked-out the repo:

```bash
git submodule update --init --recursive
```

To update the project templates:

```bash
git submodule update --remote rails/app
```

To pull, with submodules in mind for safety:

```bash
git pull --recurse-submodules
```
