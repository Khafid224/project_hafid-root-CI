LAPORAN PERTEMUAN 2
[LAPORAN PENGUJIAN INSTALASI FRAMEWORK CI.pdf](https://github.com/Khafid224/project_hafid-root-CI/files/14442912/LAPORAN.PENGUJIAN.INSTALASI.FRAMEWORK.CI.pdf)

Screnshot
![image](https://github.com/Khafid224/project_hafid-root-CI/assets/145306005/dd9552ca-ce77-4a49-9141-12409aec645d)
![image](https://github.com/Khafid224/project_hafid-root-CI/assets/145306005/2c99fd0c-7f25-4e24-b58a-2d4a98c36fcf)
![image](https://github.com/Khafid224/project_hafid-root-CI/assets/145306005/c60b1a3b-47b3-47b8-85e9-2b340e9acdf4)
![image](https://github.com/Khafid224/project_hafid-root-CI/assets/145306005/c19c5fdb-d463-4470-a3dc-9fcc4c305440)
![image](https://github.com/Khafid224/project_hafid-root-CI/assets/145306005/49c6f58f-3b54-4ba3-8e2b-cec1b0e3f0bb)


# CodeIgniter 4 Application Starter

## What is CodeIgniter?

CodeIgniter is a PHP full-stack web framework that is light, fast, flexible and secure.
More information can be found at the [official site](https://codeigniter.com).

This repository holds a composer-installable app starter.
It has been built from the
[development repository](https://github.com/codeigniter4/CodeIgniter4).

More information about the plans for version 4 can be found in [CodeIgniter 4](https://forum.codeigniter.com/forumdisplay.php?fid=28) on the forums.

You can read the [user guide](https://codeigniter.com/user_guide/)
corresponding to the latest version of the framework.

## Installation & updates

`composer create-project codeigniter4/appstarter` then `composer update` whenever
there is a new release of the framework.

When updating, check the release notes to see if there are any changes you might need to apply
to your `app` folder. The affected files can be copied or merged from
`vendor/codeigniter4/framework/app`.

## Setup

Copy `env` to `.env` and tailor for your app, specifically the baseURL
and any database settings.

## Important Change with index.php

`index.php` is no longer in the root of the project! It has been moved inside the *public* folder,
for better security and separation of components.

This means that you should configure your web server to "point" to your project's *public* folder, and
not to the project root. A better practice would be to configure a virtual host to point there. A poor practice would be to point your web server to the project root and expect to enter *public/...*, as the rest of your logic and the
framework are exposed.

**Please** read the user guide for a better explanation of how CI4 works!

## Repository Management

We use GitHub issues, in our main repository, to track **BUGS** and to track approved **DEVELOPMENT** work packages.
We use our [forum](http://forum.codeigniter.com) to provide SUPPORT and to discuss
FEATURE REQUESTS.

This repository is a "distribution" one, built by our release preparation script.
Problems with it can be raised on our forum, or as issues in the main repository.

## Server Requirements

PHP version 7.4 or higher is required, with the following extensions installed:

- [intl](http://php.net/manual/en/intl.requirements.php)
- [mbstring](http://php.net/manual/en/mbstring.installation.php)

> [!WARNING]
> The end of life date for PHP 7.4 was November 28, 2022.
> The end of life date for PHP 8.0 was November 26, 2023.
> If you are still using PHP 7.4 or 8.0, you should upgrade immediately.
> The end of life date for PHP 8.1 will be November 25, 2024.

Additionally, make sure that the following extensions are enabled in your PHP:

- json (enabled by default - don't turn it off)
- [mysqlnd](http://php.net/manual/en/mysqlnd.install.php) if you plan to use MySQL
- [libcurl](http://php.net/manual/en/curl.requirements.php) if you plan to use the HTTP\CURLRequest library
