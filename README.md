# WPeC to WooCommerce converter

A Wordpress plugin to help migrating from WP e-Commerce to WooCommerce.

> USE AT YOUR OWN RISK!

> This is a developer's plugin. We recommend that you read the code and only use it on a test version of your site.

> BACK UP YOUR DATABASE! This plugin converts from WP e-Commerce to WooCommerce in place. This is a potentially destructive operation. The only way to recover if the conversion fails is to restore the database from a backup.

## Installation

- Install as any WP plugin (copy to `wp-content/plugins`).

- Make sure Woocommerce plugin is activated.

- Go to `Tools > WPeC to Woo` and check the numbers

- _Optional:_ Disable WP e-Commerce, (this will speed up the migration by a lot).

- Click `Convert my store` and watch the magic happen

## What it does

The plugin converts **products**, (including variations), **categories** and **orders** to WooCommerce. 

Many shop settings will be lost in the process, it also sets all products tax status to 'taxable' and the tax class to 'standard' regardless.

## What it doesn't doesn't do

- There is no refund line item on refunded orders.
- Backorder status may not be transferred properly.
- Featured products may not be transferred properly.
- Product galleries may not be transferred as expected on newer versions of WP e-Commerce.
- Order Taxes are very USA-centric.

## Notes:

- Product attributes may appear in a different order than they do in the WP e-Commerce shop.

## Compatibility

This has been tested on WP 4.8.9, using WPEC 3.13.1 and Woocommerce 3.4.7.

Please let us know if you have any issues or requests.

## Suggestions for future improvements

- Operate more on WooCommerce objects, (WC_Product, WC_Order, etc), instead of the underlying WP data.
- Improve handling of taxes on orders, (tax rates and tax totals on orders & items in orders).
- Improve handling of product galleries.
