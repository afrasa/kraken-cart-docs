# How to Set Up Free Shipping Rewards in Shopify with Kraken Cart Drawer

Offering free shipping at a specified spend threshold is a powerful way to boost average order value and encourage customers to complete purchases. In this guide, you’ll learn how to configure the Kraken Cart Drawer app so that shoppers automatically receive free shipping once their cart total reaches \$150. We’ll walk through both the Kraken Cart Drawer setup and the necessary Shopify discount configuration.

<img width="1512" alt="image" src="https://github.com/user-attachments/assets/4e47ca12-e440-4f43-a011-1ae97fc6006b" />
---

## Why Offer Free Shipping

Free shipping is one of the most effective incentives an online store can provide. When customers see that shipping drops off if they spend a certain amount, they’re more likely to add extra items to their cart. By combining Kraken Cart Drawer’s progress bar with an automatic Shopify discount, you can create a seamless experience:

1. **Kraken Cart Drawer** shows a progress bar indicating how close the cart is to the \$150 threshold.  
2. Once the threshold is met, Kraken Cart displays a “Free Shipping” reward.  
3. A matching Shopify automatic discount ensures that shipping truly becomes free at checkout.

---

## 1. Install Kraken Cart Drawer (If You Haven’t Already)

Before getting started, make sure the Kraken Cart Drawer app is installed in your Shopify store. If you haven’t installed it yet:

1. Go to the <a href="https://apps.shopify.com/kraken-cart" target="_blank" rel="noopener noreferrer">Kraken Cart Drawer listing</a> on the Shopify App Store.  
2. Click **Add app** and follow the prompts to install.  
3. Once installed, you’ll see **Kraken Cart Drawer** under the **Apps** section of your Shopify Admin.

---

## 2. Configure the Free Shipping Reward Tier

### 2.1 Open the Cart Editor

1. In **Shopify Admin**, click **Apps** in the left sidebar.  
2. Select **Kraken Cart Drawer** from the list of installed apps.  
3. In the Kraken Cart Drawer dashboard, click **Cart Editor** in the left-hand menu.  

   <img width="1505" alt="1-cart-editor" src="https://github.com/user-attachments/assets/c007dd07-d38d-4a66-984b-49562fd71b05" />
   *Screenshot: Clicking “Cart Editor” in Kraken Cart Drawer.*

### 2.2 Add a New Reward Tier

1. Within **Cart Editor**, click **Rewards** from the sidebar submenu.  
2. Scroll down and click **Add new tier** (you may need to scroll if you already have existing tiers).  
   <img width="1512" alt="2-reward-new-tier" src="https://github.com/user-attachments/assets/bdfa6df2-ac37-4032-930e-af9eabd41fb6" />
   *Screenshot: “Add new tier” button in the Rewards section.*

3. A blank reward tier will appear (If you already have a reward tier). Configure the fields as follows:  
   - **Type**: Select **Shipping**.  
   - **Total Price**: Enter **150** (so customers must spend \$150 to qualify).  
   - **Text before achieving**: Enter:
     ```
     Spend {{remaining}} more to reach free shipping
     ```
     The `{{remaining}}` placeholder dynamically displays how many dollars remain until the threshold is met.  

   <img width="1511" alt="3-free-shipping-tier" src="https://github.com/user-attachments/assets/370baf56-a629-4dd0-8bdd-7134e3dbd59f" />
   *Screenshot: Setting up a “Shipping” reward tier with the $150 threshold.*

4. Click **Save** to apply the new tier.

---

## 3. Create the Shopify Free Shipping Discount

Kraken Cart Drawer will display the progress bar and messaging, but you still need to create an actual free shipping discount in Shopify so that the cart total at checkout includes free shipping.

### 3.1 Open Shopify Discounts

1. In **Shopify Admin**, click **Discounts** in the left-hand menu.  
   <img width="1512" alt="5-free-shipping-discount" src="https://github.com/user-attachments/assets/52d4594c-e861-44ea-94c9-042052878799" />
   *Screenshot: “Discounts” link in Shopify Admin’s sidebar.*

2. Click **Create discount**, then select **Free shipping** as the discount type.  
   <img width="1511" alt="4-free-shipping-discount" src="https://github.com/user-attachments/assets/05b52142-0022-473b-a6dd-b4bda63f9874" />
   *Screenshot: Creating a “Free shipping” discount in Shopify.*

### 3.2 Configure the Free Shipping Discount

1. Choose **Automatic discount** (so it applies automatically at checkout).  
2. In the **Title** field, enter **Free Shipping** (or any name you prefer).  
3. Under **Minimum purchase requirements**, select **Minimum purchase amount** and enter **150**.  
4. In the **Combinations** section, check all boxes so this free shipping discount can stack with other promotions.  
5. Click **Save** to activate the discount.  
   <img width="1509" alt="6-free-shipping-discount" src="https://github.com/user-attachments/assets/cad11b02-541f-4ef5-8ca8-fcdc184fabe9" />
   *Screenshot: Configuring the Free Shipping discount with a $150 minimum.*

---

## 4. Verify the Free Shipping Reward

With both Kraken Cart Drawer and the Shopify discount configured, it’s time to test the setup in your storefront:

1. **Open your storefront**.
2. **Add products** to the cart until the subtotal is \$150 or more.  
3. **Open the Kraken Cart Drawer** (by clicking the cart icon or “View cart”).  
4. Confirm that the progress bar has reached the free shipping threshold and that the “Free Shipping” reward appears.  
    <img width="1511" alt="7-free-shipping-discount" src="https://github.com/user-attachments/assets/6b9e9e40-e8ca-473f-abe0-904be6caf85a" />
   *Screenshot: Kraken Cart Drawer displaying the “Free Shipping” reward in the progress bar.*

5. **Proceed to checkout**. Verify that shipping is applied at \$0.  

If everything is set up correctly, you will see shipping listed as “Free” at the bottom of the cart or in the checkout shipping options.

---

## 5. Tips and Best Practices

- **Adjust Threshold as Needed**: You can choose any spend amount (e.g., \$50, \$100, \$200) based on your business goals.  
- **Custom Messaging**: The `{{remaining}}` variable is a powerful way to motivate customers—it shows exactly how much more they need to spend to qualify.  
- **Branding & Styling**: Consider customizing the reward bar colors in Kraken Cart Drawer to match your store’s theme.  
- **Monitor Performance**: After launching the free shipping threshold, monitor your average order value and cart abandonment rates to measure the impact.  
- **Stacking Rules**: If you run multiple promotions, double-check your “Combinations” settings in Shopify Discounts to ensure free shipping can stack appropriately.

---

## Conclusion

By following these steps, you can seamlessly offer free shipping to customers who meet your spend threshold. Kraken Cart Drawer displays a clear progress bar and messaging, encouraging shoppers to add more to their cart. Simultaneously, Shopify’s automatic discount ensures that shipping truly becomes free at checkout.

- **Kraken Cart Drawer**: Manages the reward tier and displays progress.  
- **Shopify Discounts**: Applies the actual free shipping at checkout.

Together, they create a frictionless experience that boosts cart values and enhances customer satisfaction. If you have any questions, contact our support team at **support@commercewiser.com**. Happy selling and enjoy offering free shipping to your customers!  
