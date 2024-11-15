<p align="center"><img width="371" height="58" src="/art/logo.svg" alt="Logo Laravel Jetstream"></p>

<p align="center">
    <a href="https://github.com/laravel/jetstream/actions"><img src="https://github.com/laravel/jetstream/workflows/tests/badge.svg" alt="Build Status"></a>
    <a href="https://packagist.org/packages/laravel/jetstream"><img src="https://img.shields.io/packagist/dt/laravel/jetstream" alt="Total Downloads"></a>
    <a href="https://packagist.org/packages/laravel/jetstream"><img src="https://img.shields.io/packagist/v/laravel/jetstream" alt="Latest Stable Version"></a>
    <a href="https://packagist.org/packages/laravel/jetstream"><img src="https://img.shields.io/packagist/l/laravel/jetstream" alt="License"></a>
</p>

> Disclaimer: this is an **unofficial** fork of Jetstream meant to be a community-driven adding additional options for 
> projects scaffolded using Jetstream. This package is published **separately** from the official Jetstream package and 
> meant to be used as a drop in replaced. I'll do my best to keep this fork updated, but PRs are always welcome!

## Introduction

Typestream is Laravel Jetstream fork beautifully designed application scaffolding for Laravel. Jetstream provides the perfect starting point for your next Laravel application and includes login, registration, email verification, two-factor authentication, session management, API support via [Laravel Sanctum](https://github.com/laravel/sanctum), and optional team management.

Jetstream is designed using [Tailwind CSS](https://tailwindcss.com) and offers your choice of [Livewire](https://jetstream.laravel.com/stacks/livewire.html) or [Inertia](https://jetstream.laravel.com/stacks/inertia.html) scaffolding.
For those using the Inertia stack, you may optionally choose to use [TypeScript](https://www.typescriptlang.org/) as well.

Additionally for those choosing Inertia, you may also choose to install [ESLint](https://www.typescriptlang.org/) pre-configured with the [popular
Vue-based rules](https://github.com/antfu/eslint-config/) provided by Vue community member [Anthony Fu](https://antfu.me/).

## Official Documentation

Documentation for this fork of Jetstream is the same as written on the [Jetstream website](https://jetstream.laravel.com).
See the section below for instructions on getting started with the fork in place of the official package.

## Getting Started

This fork adds additional scaffolding for Jetstream with all options in the documentation fully intact. As of now,
the only enhancement is the addition of TypeScript support for the Inertia stack. To get started with this fork, simply
scaffold a new Laravel project

```bash
## Scaffold a new bare bones Laravel project
composer create-project laravel/laravel example-app

cd example-app

## IMPORTANT: install this fork _instead_ of the official laravel/jetstream package
composer require joeymckenzie/jetstream
```

Refer to the official documentation for the available artisan install commands. Typestream offers the additional `--typescript` option for Inertia stacks:

```bash
## Installs Vue-based Inertia with TypeScript support, though all other options also work
php artisan jetstream:install inertia --typescript
```

## Contributing

Thank you for considering contributing to Jetstream! You can read the contribution guide [here](.github/CONTRIBUTING.md).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

Please review [our security policy](https://github.com/laravel/jetstream/security/policy) on how to report security vulnerabilities.

## License

Laravel Jetstream is open-sourced software licensed under the [MIT license](LICENSE.md).
