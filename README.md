# Kraken Cart Drawer Technical Documents

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