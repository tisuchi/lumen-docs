# Installation

- [Installation](#installation)
    - [Server Requirements](#server-requirements)
    - [Installing Lumen](#installing-lumen)
    - [Configuration](#configuration)
- [Compatibility](#compatibility)

<a name="installation"></a>
## Installation

> **Note:** In the years since releasing Lumen, PHP has made a variety of wonderful performance improvements. For this reason, along with the availability of [Laravel Octane](https://laravel.com/docs/octane), we no longer support beginning new projects with Lumen. Instead, we recommend always beginning new projects with [Laravel](https://laravel.com).

<a name="server-requirements"></a>
### Server Requirements

The Lumen framework has a few system requirements. You will need to make sure your server meets the following requirements:

<div class="content-list" markdown="1">
- PHP >= 8.0
- OpenSSL PHP Extension
- PDO PHP Extension
- Mbstring PHP Extension
</div>

### Serving Your Application

To serve your project locally, you may use the [Laravel Homestead](http://laravel.com/docs/homestead) virtual machine, [Laravel Valet](http://laravel.com/docs/valet), or the built-in PHP development server:

    php -S localhost:8000 -t public

<a name="configuration"></a>
### Configuration

All of the configuration options for the Lumen framework are stored in the `.env` file. Once Lumen is installed, you should also [configure your local environment](/docs/{{version}}/configuration#environment-configuration).

#### Application Key

The next thing you should do after installing Lumen is set your application key to a random string. Typically, this string should be 32 characters long. The key can be set in the `.env` environment file. If you have not renamed the `.env.example` file to `.env`, you should do that now. **If the application key is not set, your user encrypted data will not be secure!**

<a name="compatibility"></a>
## Compatibility

Since Lumen is a totally separate framework from Laravel, it does not intentionally offer compatibility with any additional Laravel libraries like Cashier, Passport, Scout, etc. If your application requires the functionality provided by these libraries, please use [the Laravel framework](https://laravel.com).
