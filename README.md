

PostFinanceCheckout Payment for Shopware 6.2.3 - 6.3.*
=============================

The PostFinanceCheckout Payment plugin wraps around the PostFinanceCheckout API. This library facilitates your interaction with various services such as transactions.

## Requirements

- PHP 7.2 and above
- Shopware 6.2.3 and above

## Installation

You can use **Composer** or **install manually**

### Composer

The preferred method is via [composer](https://getcomposer.org). Follow the
[installation instructions](https://getcomposer.org/doc/00-intro.md) if you do not already have
composer installed.

Once composer is installed, execute the following command in your project root to install this library:

```bash
composer require postfinancecheckout/shopware-6-3
php bin/console plugin:refresh
php bin/console plugin:install --activate --clearCache PostFinanceCheckoutPayment
```

#### Update via composer
```bash
composer update postfinancecheckout/shopware-6-3
php bin/console plugin:refresh
php bin/console plugin:install --activate --clearCache PostFinanceCheckoutPayment
```

### Manual Installation

Alternatively you can download the package in its entirety. The [Releases](../../releases) page lists all stable versions.

Uncompress the zip file you download, and include the autoloader in your project:

```bash
# unzip to ShopwareInstallDir/custom/plugins/PostFinanceCheckoutPayment
composer require postfinancecheckout/sdk 3.0.0
php bin/console plugin:refresh
php bin/console plugin:install --activate --clearCache PostFinanceCheckoutPayment
```

## Usage
The library needs to be configured with your account's space id, user id, and application key which are available in your PostFinanceCheckout
account dashboard.

### Logs and debugging
To view the logs please run the command below:
```bash
cd shopware/install/dir
tail -f var/log/postfinancecheckout_payment*.log
```

## Documentation

[Documentation](https://plugin-documentation.postfinance-checkout.ch/pfpayments/shopware-6-3/3.1.1/docs/en/documentation.html)

## License

Please see the [license file](https://github.com/pfpayments/shopware-6-3/blob/master/LICENSE.txt) for more information.