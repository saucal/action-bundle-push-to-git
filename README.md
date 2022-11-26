# BUNDLE: Push to GIT

This action is a bundle of other actions which simplifies the workflow definition process for our standard wp-content rooted projects.

## Getting Started

This is the most common configuration

```yml
- name: Push to GIT
  uses: saucal/action-bundle-push-to-git@v1
```

## Full options

```yml
- uses: saucal/action-bundle-push-to-git@v1
  with:
    # Folder where source code is already built
    source: "source"

    # Folder of the repo that things will be pushed to
    built: "built"

    # Token to use throughout the process
    force-ignore: |
      /vendor/*
      !/vendor/composer
      /vendor/composer/*
      !/vendor/composer/installers
      !/vendor/composer/installed.json
```
