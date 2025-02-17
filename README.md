# Mink WebDriver Classic Driver

[![Latest Stable Version](https://poser.pugx.org/mink/webdriver-classic-driver/v)](https://packagist.org/packages/mink/webdriver-classic-driver)
[![Latest Unstable Version](https://poser.pugx.org/mink/webdriver-classic-driver/v/unstable)](https://packagist.org/packages/mink/webdriver-classic-driver)
[![Total Downloads](https://poser.pugx.org/mink/webdriver-classic-driver/downloads)](https://packagist.org/packages/mink/webdriver-classic-driver)
[![CI](https://github.com/minkphp/webdriver-classic-driver/actions/workflows/ci.yml/badge.svg)](https://github.com/minkphp/webdriver-classic-driver/actions/workflows/ci.yml)
[![License](https://poser.pugx.org/mink/webdriver-classic-driver/license)](https://github.com/minkphp/webdriver-classic-driver/blob/main/LICENSE)
[![codecov](https://codecov.io/gh/minkphp/webdriver-classic-driver/branch/main/graph/badge.svg?token=11hgqXqod9)](https://codecov.io/gh/minkphp/webdriver-classic-driver)

## Installation

``` bash
composer require behat/mink mink/webdriver-classic-driver
```

## Testing

1. Start WebDriver
    1. If you have Docker installed, run
    ```bash
    docker run -p 4444:4444 selenium/standalone-firefox:2.53.1
    ```
    2. If you do not have Docker, but you have Java
    ```bash
    curl -L https://selenium-release.storage.googleapis.com/2.53/selenium-server-standalone-2.53.1.jar > selenium-server-standalone-2.53.1.jar
    java -jar selenium-server-standalone-2.53.1.jar
    ```
2. Start WebServer by running
    ``` bash
    ./vendor/bin/mink-test-server
    ```
3. Start PhpUnit
    ```bash
    ./vendor/bin/phpunit -v --coverage-clover=coverage.clover
    ```
