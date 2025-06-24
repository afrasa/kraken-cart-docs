# Kraken Cart Drawer Technical Documents

### Table of Contents
- [How to install Kraken Cart App from the App Store link](#how-to-install-kraken-cart-app-from-the-app-store-link)
- [How to resize cart drawer for desktop devices](#how-to-resize-cart-drawer-for-desktop-devices)
- **How to setup rewards**
  - [How to use the Free Shipping Bar](../blog/rewards/free-shipping-bar.md)

### How to install Kraken Cart App from the App Store link
- Visit [Kraken Cart](https://apps.shopify.com/kraken-cart) page on Shopify app store.
- Click the "Install" button on the app page.
- Follow the on-screen instructions to authorize the app for your store.

### How to resize cart drawer for desktop devices
- Open Kraken Cart App on your store
- Open Cart Editor
- Select "Settings"
- Paste the following style into the custom style section and adjust the numbers:
```css
@media (min-width: 768px) {
    .drawer-sheet {
        width: 435px;
    }
}
@media (min-width: 640px) {
    .drawer-sheet {
         max-width: 448px;
    }
}
```
<img width="1512" alt="image" src="https://github.com/user-attachments/assets/4e47ca12-e440-4f43-a011-1ae97fc6006b" />