<p align="center">
  <img src="https://raw.githubusercontent.com/laradock/laradock/master/.github/home-page-images/laradock-logo.png" alt="Laradock Logo" width="640">
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

This is the base image for the Laradock **PHP-FPM** container, the PHP runtime that serves your application behind a web server such as Nginx, Apache, or Caddy.

It ships a clean, configurable PHP-FPM process with the extensions a typical PHP app needs, and lets you switch PHP versions in one place so each project runs on exactly the runtime it expects. Together with the Workspace image it forms the core of a Laradock stack, with nothing installed on your host.

Images are built and published automatically to [Docker Hub](https://hub.docker.com/r/laradock/php-fpm) for each supported PHP version.

## Links

* 📖 [Documentation](https://laradock.io)
* 📦 [Laradock main repository](https://github.com/laradock/laradock)
* 🐳 [Docker Hub](https://hub.docker.com/r/laradock/php-fpm)
* 🤝 [Contribution guide](https://laradock.io/contributing)
* ✏️ [Editing base images](https://laradock.io/contributing/#edit-base-image)

## License

[MIT](https://github.com/laradock/laradock/blob/master/LICENSE)
