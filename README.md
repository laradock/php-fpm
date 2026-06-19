<p align="center">
  <img src="https://raw.githubusercontent.com/laradock/laradock/master/.github/home-page-images/laradock-logo.png" alt="Laradock Logo" width="800">
</p>

<h1 align="center">Laradock PHP-FPM Image</h1>

<p align="center">
  The PHP-FPM base image for <a href="https://github.com/laradock/laradock">Laradock</a>, the runtime that serves your PHP application.
</p>

<p align="center">
  <a href="https://github.com/laradock/php-fpm/actions/workflows/dockerimage.yml"><img src="https://github.com/laradock/php-fpm/actions/workflows/dockerimage.yml/badge.svg" alt="Docker Image CI"></a>
  <a href="https://hub.docker.com/r/laradock/php-fpm"><img src="https://img.shields.io/docker/pulls/laradock/php-fpm.svg" alt="Docker Pulls"></a>
  <a href="https://raw.githubusercontent.com/laradock/laradock/master/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a>
</p>

## About

This repository builds and publishes the **PHP-FPM** base image used by [Laradock](https://github.com/laradock/laradock). It exists on its own so the image can be prebuilt and shipped to Docker Hub, which keeps Laradock builds fast on your machine instead of compiling PHP and its extensions locally every time.

PHP-FPM is the PHP runtime that serves your application behind a web server such as Nginx, Apache, or Caddy. This image ships a clean, configurable PHP-FPM process with the extensions a typical PHP app needs, and lets you switch PHP versions in one place so each project runs on exactly the runtime it expects. Together with the Workspace image it forms the core of a Laradock stack, with nothing installed on your host.

Images are built and published automatically to [Docker Hub](https://hub.docker.com/r/laradock/php-fpm) for each supported PHP version.

## Usage

You normally use this image through Laradock rather than directly, but you can pull it on its own:

```bash
docker pull laradock/php-fpm:latest-8.4
```

## Links

* 📖 [Documentation](https://laradock.io)
* 📦 [Laradock main repository](https://github.com/laradock/laradock)
* 🐳 [Docker Hub](https://hub.docker.com/r/laradock/php-fpm)
* 🤝 [Contribution guide](https://laradock.io/contributing)
* ✏️ [Editing base images](https://laradock.io/contributing/#edit-base-image)

## License

MIT © [Mahmoud Zalt](https://zalt.me)
