# Introduction #

The goal of this connector is to allow you to use the best of both tools without having to manually transfer data from one to the other. We are not intending to have one single interface to control both tools. So when using this connector, you will still need to use both interfaces. Our goal is not to control all Magento features from OpenERP or vice versa.

The following points will describe how to be efficient with this connector. For each task we explain what we think is the best way to achieve it. You may of course use it the way you want, but at least you know what we had in mind when we designed it.


# 1. Working with product categories #

Categories can be created or modified in Magento or OpenERP. You can then import the categories you have configured in Magento into OpenERP or you can export the categories you have configured in OpenERP to Magento.

When importing or exporting products, categories are also imported or exported.

In Magento, it is not mandatory for a product to be assigned to a category while it OpenERP it is. This is why, when configuring your Magento Store in OpenERP, you need to specify a default category. This category will be used for products that have no categories in Magento.


# 2. Working with products #

There are only a few parameters that are synchronized between OpenERP and Magento. At this point they are :
  * Name
  * Code / SKU
  * Price
  * Weigth
  * Stock

When creating new products, it is recommended to create it first into Magento like you would do with a single Magento installation. Then, you can import it into OpenERP.

Once the product is in both Magento and OpenERP, you can start using OpenERP for your day-to-day product management (stock, purchase orders to your supplier, production...)

For the Magento parameters (pictures, descriptions, tax classes, ...) you should keep using the Magento interface.
In the future we may include more stuff in OpenERP like tax classes, but all parameters that are really specific to the online store like descriptions and pictures will stay in Magento (we do not see, at this point, any added value to moving this to OpenERP).


# 3. Working with orders and invoices #


TODO