# How to hide the “Shipping Protection” product from *Featured Collection* section

## ✅ What You'll Do

You’ll edit the `featured-collection.liquid` section to **exclude** any product with the title “Shipping Protection” so it doesn’t appear in product grids or sliders.

---

## 🧱 Step-by-Step Guide

### 🔁 1. Duplicate Your Live Theme

1. Go to your Shopify admin.
2. Navigate to **Online Store > Themes**.
3. Under your **Current theme**, click **••• > Duplicate**.
4. Your duplicate will appear in the **Theme Library** — click **Rename** to call it something like `Dawn – test edits`.

---

### 🔍 2. Open the Code Editor

1. Next to your duplicate theme, click **Actions > Edit code**.
2. In the **Sections** folder, open:
   `featured-collection.liquid`
   (or it may be named `main-collection-product-grid.liquid` depending on your version of Dawn).

---

### ✏️ 3. Add the Filtered Product List

Find the section at the top that begins with:

```liquid
{%- liquid
  assign products_to_display = section.settings.collection.all_products_count
```

➡️ Just **above that**, add this:

```liquid
{%- assign filtered_products = section.settings.collection.products 
    | reject: "title", "Shipping Protection" -%}
```

This creates a filtered version of the collection’s products, excluding any titled exactly `"Shipping Protection"`.

---

### 🔁 4. Update the Product Loop

Search for this line (your product loop):

```liquid
{% for product in section.settings.collection.products limit: section.settings.products_to_show %}
```

Replace it with:

```liquid
{% for product in filtered_products limit: section.settings.products_to_show %}
```

✅ That tells Shopify to only loop through the filtered list.

---

### 🔢 5. (Optional) Fix the “View All” & Counter Logic

If you want to make sure your **slider counter** and **"View All"** logic respects the filtered product count, replace:

```liquid
assign products_to_display = section.settings.collection.all_products_count
```

with:

```liquid
assign products_to_display = filtered_products.size
```

Then the counter and "View All" link won’t be triggered by hidden items.

---

### 💾 6. Save and Preview

1. Click **Save** in the top-right corner.
2. Go back to **Themes > Theme Library**.
3. Click **Preview** on your duplicated theme.
4. Navigate to a page that shows a **Featured Collection** section — the “Shipping Protection” product should now be gone.

---

## ✅ Done!

You’ve now successfully hidden the “Shipping Protection” product from your featured collection section — without affecting your actual product catalog or inventory.
