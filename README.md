# BDC_Core

This module is used as a wrapper for all BDCrops Magento 2 extensions.



## How to install & upgrade BDC_Core


### 1. Copy and paste

If you don't want to install via composer, you can use this way.

- Download [the latest version here](https://github.com/bdcrops/module-core/archive/master.zip)
- Extract `master.zip` file to `app/code/BDC/Core` ; You should create a folder path `app/code/BDC/Core` if not exist.
- Go to Magento root folder and run upgrade command line to install `BDC_Core`:

```
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```




[![Latest Stable Version](https://poser.pugx.org/bdcrops/module-core/v/stable)](https://packagist.org/packages/bdcrops/module-core)
[![Total Downloads](https://poser.pugx.org/bdcrops/module-core/downloads)](https://packagist.org/packages/bdcrops/module-core)



### 2. Install via composer

We recommend you to install BDC_Core module via composer. It is easy to install, update and maintaince.

Run the following command in Magento 2 root folder.

#### 2.1 Install

Run
```
composer config repositories.module-core git
https://github.com/bdcrops/module-core.git

composer require bdcrops/module-core:~1.0.0
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```

#### 2.2 Upgrade

```
composer update bdcrops/module-core
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```

Run compile if your store in Product mode:

```
php bin/magento setup:di:compile
