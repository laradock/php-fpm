# AGENTS.md

Guidance for AI agents and contributors working in this repository.

## What this is

This repository builds and publishes the **PHP-FPM** base image used by [Laradock](https://github.com/laradock/laradock): the PHP runtime that serves an application behind Nginx, Apache, or Caddy. It is not application code; it exists so the image can be prebuilt once and pulled from Docker Hub instead of compiled locally on every Laradock `docker-compose build`.

## How it works

- One `Dockerfile-<php-version>` per supported PHP version at the repo root.
- No Makefile here (unlike the sibling `workspace` repo), build a version directly: `docker build -f Dockerfile-8.4 -t php-fpm:dev-8.4 .`
- CI (`.github/workflows/dockerimage.yml`) builds and pushes to Docker Hub (`laradock/php-fpm`) via a version matrix. Older versions (5.6-7.3) are currently commented out of that matrix, check it before assuming a version is still built.
- No separate test suite, a successful multi-arch build is the check.

## Conventions

- Keep each `Dockerfile-<version>` self-contained and consistent with its siblings.
- This image is pulled directly from Docker Hub by users as well as by `laradock/laradock`. Treat changes as public-API changes: additive, and build-test the specific version(s) you touch.

## Docs

- Full documentation: https://laradock.io
- Contribution guide: https://laradock.io/contributing
- Editing base images: https://laradock.io/contributing/#edit-base-image
