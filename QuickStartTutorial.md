# 1. Installation #

Before starting this tutorial, please make sure you have installed the Magento module and the OpenERP extension.

See our [Installation](Installation.md) page for help.


# 2. Create a Magento Store #

  1. Create a default category if none exists. This will be your default category for products that have no category in Magento.
  1. Create a Shipping product if none exists. This product will be used for shipping costs for imported orders from Magento.
  1. Go to the _Magento_ / _Magento Settings_ and create a new Magento store.
  1. Choose a name.
  1. Enter the Base URL where your Magento store is installed (the URL to reach the main page).
  1. Enter the _API User_ and _API Key_ you configured during the Magento module installation (see [Installation](Installation.md)).
  1. Select your _default category_ and default _shipping product_.
  1. `[`Optional`]` If you want to use accounting in OpenERP, you may want to choose a _Payment Journal_.
  1. You may leave _Automatic Synchronization Settings_ to default values for now.

At this time, only one store is supported.


# 3. Import categories and product from Magento #

> Once you are done with step 2, you are ready to import