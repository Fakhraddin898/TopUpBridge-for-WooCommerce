# FX TopUpEpin for WooCommerce

A WordPress plugin that integrates the **TopUpEpin B2B API** with WooCommerce — sync products, manage category images, handle game info fields at checkout, and submit orders directly to the TopUpEpin API.

---

## Features

- **API Integration** — Connect your WooCommerce store to the TopUpEpin B2B API (`https://topupepin.com/api/v1`)
- **Product Sync** — Import and synchronize TopUpEpin products into WooCommerce automatically
- **Category Images** — Automatically assign images to products based on their TopUpEpin category
- **Game Info at Checkout** — Adds custom game-specific fields (e.g. Player ID, Server ID) to the WooCommerce checkout
- **Order Submission** — Sends WooCommerce orders to the TopUpEpin API in real time
- **Cleanup Tool** — Bulk delete all synced TopUpEpin products when needed
- **IPv4 Forced Requests** — Ensures all API calls use IPv4 for maximum compatibility

---

## Requirements

- WordPress 5.6+
- WooCommerce 5.0+
- PHP 7.4+
- A valid TopUpEpin B2B API account

---

## Installation

1. Download the latest release (`fx-topupepin.zip`) from the [Releases](../../releases) page.
2. In your WordPress admin panel, go to **Plugins → Add New → Upload Plugin**.
3. Upload the zip file and click **Install Now**, then **Activate**.
4. Go to **WooCommerce → TopUpEpin Settings** and enter your API credentials.

---

## Configuration

After activation, navigate to the plugin settings page and provide:

| Setting | Description |
|---|---|
| API Base URL | Default: `https://topupepin.com/api/v1` |
| API Key / Token | Your TopUpEpin B2B account credentials |
| Sync Options | Choose which product categories to import |

---

## Usage

### Sync Products
Go to the plugin admin page and click **Sync Products** to import all available TopUpEpin products into WooCommerce.

### Checkout Fields
Game-specific fields are automatically added to checkout for TopUpEpin products (e.g. User ID, Zone/Server). These are sent with the order to the API.

### Cleanup
Use the **Clean TopUpEpin Products** button to remove all synced products and their images from WooCommerce.

---

## Changelog

### v1.9.3
- Initial public release
- Full B2B API integration
- Product sync with category image support
- Checkout game info fields
- Order submission to TopUpEpin API
- IPv4 enforcement for cURL and stream requests

---

## Author

**Fakhraddin Ahmadov** (Faxri) — built with assistance from ChatGPT.

---

## License

This project is released for personal and commercial use. Please review the [TopUpEpin API Terms of Service](https://topupepin.com) before deploying in production.
