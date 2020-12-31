# About DE

This project a beta version of our docker env for local and production work. Because of changes with technologies which we would have used, we may make drastic changes.

# <span style="color:#007bff"> Table of content </span>

- [About DE](#about-de)
- [<span style="color:#007bff"> Table of content </span>](#-table-of-content-)
  - [Prerequisites](#prerequisites)
    - [Technologies](#technologies)
    - [Setup Environment for Development:](#setup-environment-for-development)
    - [Setup Environment for Production:](#setup-environment-for-production)
  - [License](#license)

## Prerequisites

---
Insall:

-   `Docker` - [Download & install Docker](https://docs.docker.com/get-docker/)  - make sure that the latest docker version has been installed on your machine.

### Technologies

---

List of technologies which are used in this project.

-   PHP : Version 7.4
-   MySQL: Version 8
-   Node: Version 14.15.0

### Setup Environment for Development:

-   Copy `.env.example` to `.env`.
-   Build `docker-compose build`.
-   Run `docker-compose up -d` for development purpose.
-   Open favourite browser and type `http://localhost`. If you wan to run on different port, you can change the `HTTP_PORT` from `.env` file.
-   Generate key `docker exec bakend-end php artisan key:generate`
-   If you want to install a npm package then run `docker exec front-end npm install <Package_Name>`.
-   If you want to install compose package then run `docker exec back-end compose install <PACKAGE_NAME>`.

### Setup Environment for Production:

-   Copy `.env.example` to `.env`.
-   Change the necessary staff in `.env` file.
-   Run `docker-compose -f docker-compose.production.yml up` for production.
-   Open favourite browser and type `http://localhost`. If you wan to run on different port, you can change the `HTTP_PORT` from `.env` file.
-   If you want to install a npm package then run `docker exec front-end npm install <Package_Name>`.
-   If you want to install compose package then run `docker exec back-end compose install <PACKAGE_NAME>`.


## License

The theme is available as open source under the terms of the [MIT License](LICENSE.txt).
