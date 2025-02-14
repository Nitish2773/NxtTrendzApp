---

# NxtTrendz Shopping Cart Website

## 🚀 Live Demo
[Click here to experience NxtTrendz](https://nitishnxttrendz.ccbp.tech/)

NxtTrendz is a next-generation e-commerce platform designed to provide users with a seamless and engaging online shopping experience. With a sleek interface, intuitive navigation, and advanced features, shopping has never been easier.

---

## ✨ Key Features
- 🛒 **Shopping Cart** – Effortlessly add, remove, and update product quantities.
- 🔍 **Search Functionality** – Quickly locate products with a responsive search bar.
- 🏷 **Category Browsing** – Browse through different product categories (electronics, fashion, home goods, etc.).
- 🔄 **Filtering & Sorting** – Apply filters (price range, brand) and sort by price, popularity, or ratings.
- 📄 **Product Details** – View detailed product information, including description, availability, pricing, and reviews.
- 🔗 **Similar Products** – Discover related products based on your selected item.

---

## 🎨 Responsive Design
NxtTrendz is designed to be fully responsive across all devices. Below are design previews for different screen sizes:

- 📱 **Small Screens (<576px)**:  
  ![Small Screen](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-sm-output-v0.png)

- 💻 **Medium to Large Screens (≥768px)**:  
  ![Large Screen](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-lg-output.png)

---

## ⚡ Getting Started
Follow these steps to set up and run the project locally:

### 1️⃣ Prerequisites
Ensure you have the following installed on your machine:
- Node.js
- npm (Node Package Manager)

### 2️⃣ Installation
Clone the repository and install dependencies:
```sh
npm install
```

### 3️⃣ Running the App
Start the development server:
```sh
npm start
```
The application will run at `http://localhost:3000/`.

---

## 🛍 Features to Implement

### 🔐 Authentication & Cart Access
- Users must log in before accessing the cart. Unauthenticated users will be redirected to the **Login** page.

### 🛒 Cart Functionalities
- Adding the same product multiple times increases its quantity instead of duplicating it.
- The **Cart Route** displays the total amount and item count.
- **Item Quantity Controls:**
  - Clicking **+** increases the quantity.
  - Clicking **−** decreases the quantity (removes the item if quantity is 1).
  - **Remove** button deletes an item from the cart.
  - **Remove All** button clears the entire cart.
- The product price and **Cart Summary** update dynamically.

### 🏗 Cart Context Methods
The following methods manage cart operations:
```js
cartList // Stores cart items
removeAllCartItems() // Clears all items from the cart
addCartItem(item) // Adds an item to the cart
removeCartItem(id) // Removes an individual item
incrementCartItemQuantity(id) // Increases item quantity
decrementCartItemQuantity(id) // Decreases item quantity
```

---

## 🏛 Components Structure
To understand the component architecture, refer to the image below:

![Component Structure](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-component-structure-breakdown.png)

---

## 📂 Implementation Files
The following files need updates or creation:
- `src/App.js`
- `src/components/Cart/index.js`
- `src/components/Cart/index.css`
- `src/components/CartItem/index.js`
- `src/components/CartItem/index.css`
- `src/components/CartSummary/index.js`
- `src/components/CartSummary/index.css`

---

## 💡 Quick Tips

### CSS – Line Height
Use `line-height` to control text spacing:
```css
line-height: 1.5;
```

### JavaScript – Array `find()` Method
Retrieve a specific item from an array:
```js
const item = arr.find(item => item.name === 'Product');
```

---

## 🎨 UI Elements & Icons
- **Icons (react-icons):**
  - ➕ **Plus:** `BsPlusSquare`
  - ➖ **Minus:** `BsDashSquare`
  - ❌ **Remove:** `AiFillCloseCircle`

- **Test IDs:**
  - `plus` and `minus` for cart item quantity buttons.
  - `remove` for the remove button.

---

## 🛡 User Credentials (For Testing)

### 🔑 Prime User
- **Username:** `rahul`
- **Password:** `rahul@2021`

### 🔑 Non-Prime User
- **Username:** `nitish`
- **Password:** `nitish@2021`

---

## 🎨 Design Guidelines

### 🎨 Colors Used
- ![#0b69ff](https://www.colorhexa.com/0b69ff.png) `#0b69ff`
- ![#171f46](https://www.colorhexa.com/171f46.png) `#171f46`
- ![#616e7c](https://www.colorhexa.com/616e7c.png) `#616e7c`
- ![#ffffff](https://www.colorhexa.com/ffffff.png) `#ffffff`

### 🖋 Font Used
- **Roboto**

---

## 📌 Notes
- Place all components inside `src/components`.
- Maintain the given folder structure to ensure compatibility with test cases.

---

