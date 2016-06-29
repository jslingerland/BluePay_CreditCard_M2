# BluePay_CreditCard_M2
BluePay Credit Card payment module for Magento 2. If you are looking for the Magento 1.x.x.x payment module, [Click here](https://www.magentocommerce.com/magento-connect/bluepay-creditcard-2-1.html)

Since this module links your Magento store to the BluePay gateway, a gateway account is required. [Click here](https://www.bluepay.com/contact-us/get-started/) to start the sign up process.


# Installation
1. First, navigate to your Magento 2 root directory
2. Enter the following commands:

```cmd
composer config repositories.bluepay_creditcard git https://github.com/jslingerland/BluePay_CreditCard_M2.git
composer require bluepay/creditcard:dev-master
```

Once the dependencies have finished installing, enter the next commands:

```cmd
php bin/magento module:enable BluePay_CreditCard --clear-static-content
php bin/magento setup:upgrade
```

At this point, the module should be fully installed. Finally, log into your Magento admin section and navigate to Stores -> Configuration -> Sales -> Payment Methods -> BluePay (Credit Card) to finish the setup.
