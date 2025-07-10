# Customize Kraken Cart drawer
To setup following style, Open Kraken Cart app in your shopify admin > Cart editor > Settings > Custom > Custom CSS and paste the custom styles in the box.

### How to hide the drawer footer when it's empty
```css
.drawer-sheet.empty-cart .cart-footer {
  display: none;
}
```

### How to hide variants in the cart drawer
```css
.variant {
  display: none !important;
}
```

### How to resize cart drawer for desktop devices
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