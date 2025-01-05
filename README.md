---

# NxtTrendz Shopping Cart Website

[Live Demo](https://nitishnxttrendz.ccbp.tech/)

**NxtTrendz** is an advanced e-commerce platform designed to enhance the online shopping experience. The website offers a seamless user interface and a variety of features to ensure an enjoyable shopping journey. 

### Key Features:
- **Add to Cart**: Effortlessly add items to the cart, update quantities, or remove them as needed.
- **Search Functionality**: Quickly find products using the search bar.
- **Category Browsing**: Shop by product categories (e.g., electronics, fashion, home goods).
- **Filtering Options**: Apply filters like price range and brand to refine search results.
- **Sorting Capabilities**: Sort items based on price, popularity, and ratings.
- **Product Details**: View comprehensive information about each product (description, availability, price, reviews).
- **Similar Products**: Explore related products based on the selected item.

### Design Files:
Click to view the designs for different screen sizes:
- [Extra Small and Small (Size < 576px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-sm-output-v0.png)
- [Medium, Large, and Extra Large (Size >= 768px)](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-lg-output.png)

### Setup Instructions:
1. Download dependencies:  
   Run `npm install` in your project directory.
2. Start the app:  
   Use `npm start` to launch the app.

### Features to Implement:

1. **Authentication & Cart Access:**
   - Unauthenticated users trying to access the **Cart** route will be redirected to the **Login** page.

2. **Cart Features:**
   - When the user adds the same product multiple times, the quantity should be updated, and the total cart item count should remain unchanged.
   - The **Cart Route** should display the total amount and the number of items in the cart.
   - In the **Cart Route**:
     - Clicking the plus icon should increase the quantity by one.
     - Clicking the minus icon should decrease the quantity by one.
     - If the quantity is one and the minus icon is clicked, the item should be removed from the cart.
     - The product price and **Cart Summary** should update accordingly.
   - Clicking the **Remove** button on any cart item should remove the item from the cart.
   - Clicking the **Remove All** button should clear all items from the cart and show the [Empty Cart View](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-empty-cart-view.png).

3. **Cart Context Methods:**
   - `cartList`: Stores the cart items.
   - `removeAllCartItems`: Removes all items from the cart.
   - `addCartItem`: Adds an item to the cart.
   - `removeCartItem`: Removes an individual item from the cart.
   - `incrementCartItemQuantity`: Increases the quantity of a product in the cart.
   - `decrementCartItemQuantity`: Decreases the quantity of a product in the cart.

### Components Structure:
For an overview of how the components are structured, refer to the image below:

![Component Structure](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-component-structure-breakdown.png)

### Implementation Files:
The following files need to be updated or created for the implementation:
- `src/App.js`
- `src/components/Cart/index.js`
- `src/components/Cart/index.css`
- `src/components/CartItem/index.js`
- `src/components/CartItem/index.css`
- `src/components/CartSummary/index.js`
- `src/components/CartSummary/index.css`

### Quick Tips:

- **Line Height**: The `line-height` CSS property sets the height of a line box. You can use it to set the distance between lines of text.

  Example:
  ```css
  line-height: 1.5;
  ```

- **Array Method `find()`**: The `find()` method returns the first item in an array that satisfies the provided testing function.

  Example:
  ```javascript
  const item = arr.find(item => item.name === 'Product');
  ```

### Important Notes:
- The app should use `react-icons` for buttons:
  - **Plus Icon**: `BsPlusSquare`
  - **Minus Icon**: `BsDashSquare`
  - **Remove Icon**: `AiFillCloseCircle`
  
- **Test IDs**:
  - Cart Item buttons should have the test IDs **plus** and **minus** for plus and minus actions.
  - The Cart Item **remove** button should have the test ID `remove`.

### Prime User Credentials:
- Username: `rahul`
- Password: `rahul@2021`

### Non-Prime User Credentials:
- Username: `nitish`
- Password: `nitish@2021`

### Colors Used:
- ![#0b69ff](https://www.colorhexa.com/0b69ff.png) `#0b69ff`
- ![#171f46](https://www.colorhexa.com/171f46.png) `#171f46`
- ![#616e7c](https://www.colorhexa.com/616e7c.png) `#616e7c`
- ![#ffffff](https://www.colorhexa.com/ffffff.png) `#ffffff`

### Font Used:
- **Roboto**

### Notes:
- All components should be placed in the `src/components` directory.
- Do not modify the folder names as the tests expect these exact names.

---
