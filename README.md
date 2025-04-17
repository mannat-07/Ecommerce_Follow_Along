**Ecommerce Follow Along Project**

---

### **Milestone 1: Project Overview**

- Introduction to the MERN Stack structure.
- Set up environment for future milestones.
- Created a new repository for the follow-along project.

---

### **Milestone 2: Project Setup**

- **Organize Project:** Separate into frontend and backend folders.
- **Set up React Frontend:** Create a React app for the user interface.
- **Set up Node.js Backend:** Build a basic Node.js server.
- **Configure Tailwind CSS:** Add for easy, modern styling.
- **Build Login Page:** Design and develop the first page of the app.

---

### **Milestone 3: Backend Setup**

- Organize backend code into dedicated folders.
- Initialize Node.js server and set up MongoDB connection.
- Implement basic error handling.
- Update README to document progress.

---

### **Milestone 4: User Authentication**

- **Create User Model:** Understand the MVC architecture and database interaction.
- **Create User Controller:** Learn about controller's role in MVC.
- **Enable and Configure Multer:** Set up Multer for handling file uploads.

---

### **Milestone 5: User Registration**

- **Create Sign-Up Page:** Design a page for user registration (Name, Email, Password).
- **Implement Form Validation:** Ensure correct data (valid email, secure password).
- **Build Frontend:** Use HTML and CSS for design.
- **Document Progress:** Update the README.

---

### **Milestone 6: Secure Password Storage**

- **Encrypt Password with bcrypt:** Hash passwords during signup.
- **Save Hashed Password in Database:** Store only the hashed password.
- **Store Complete User Data:** Securely store user info along with the hashed password.
- **Login with Hashed Password:** Use bcrypt to verify entered passwords during login.

---

### **Milestone 7: Login Authentication**

- **Validate User Login:** Ensure proper login credentials validation.
- **Why Encrypt Passwords:** Discuss security, privacy, and compliance.
- **Login Authentication Process:** Use bcrypt to compare hashed passwords.

---

### **Milestone 8: Product Card Creation**

- **Create Product Card Component:** Display products visually and clearly.
- **Reusable Design:** Create a card component for multiple products.
- **Layout:** Set up a grid or flexbox layout for displaying products.

---

### **Milestone 9: Product Form**

- **Create Product Form:** Allow multiple product images to be uploaded.

---

### **Milestone 10: Product Schema**

- **Write Product Schema:** Define the structure for product data.
- **Create Endpoint to Store Product Details:** Store product data in MongoDB.

---

### **Milestone 11: Display Products**

- **Create Endpoint to Fetch Product Data:** Extract and send data from MongoDB.
- **Display Data Dynamically:** Use the product card component to render products.

---

### **Milestone 12: Filter and Display Products**

- **Write Endpoint to Filter Products:** Filter product data by email and send from MongoDB.
- **Display Filtered Data on Frontend:** Render products using dynamic cards.

---

### **Milestone 13: Update Product Data**

- **Update Data in MongoDB:** Write endpoint to update product details.
- **Edit Product Button:** Allow product data to be edited.
- **Autofill Form:** Pre-fill product data for editing.

---

### **Milestone 14: Delete Product**

- **Create Endpoint to Delete Products:** Delete product data from MongoDB using ID.
- **Delete Button on Product Card:** Send product ID to the server for deletion.

---

### **Milestone 15: Navigation Component**

- **Build Nav Component:** Add links (Home, My Products, Add Product, Cart).
- **Make Responsive:** Ensure navigation works across pages.

---

### **Milestone 16: Product Detail Page**

- **Create Product Detail Page:** Display product details.
- **Select Quantity and Add to Cart:** Add functionality to select quantity and add product to cart.

---

### **Milestone 17: Cart Schema**

- **Create Cart Schema:** Design a schema to store product details in the cart.
- **Write Endpoint for Cart Data:** Store and retrieve cart data from MongoDB.

---

### **Milestone 18: Cart Page Backend**

- **Create Endpoint for Cart Page:** Retrieve products in the cart for the user.

---

### **Milestone 19: Cart Frontend and Quantity Update**

- **Create Cart Frontend Page:** Display products in the cart with product name, price, and total price.
- **Quantity Adjustment:** Include "+" and "-" buttons to adjust the product quantity.
- **Update Total Price:** Ensure the total updates as the quantity changes.
- **Backend Endpoints for Quantity Update:**
  - Increase/Decrease Quantity endpoints.
  - Ensure quantity doesn't go below 1.
- **Frontend Communication:** Use AJAX/Fetch to dynamically update the cart.

---

### **Milestone 20: User Profile and Email**

- **Create Backend Endpoint to Send User Data via Email:** Send user data (profile photo, name, email, addresses) to user's email.
- **Create Profile Page:** Display user profile (photo, name, email) and address list.
- **Add Address Button:** Allow the user to add new addresses.
- **Handle Missing Data:** Display "No address found" if no addresses exist.
- **Test Functionality:** Verify profile page and email functionality.

---

### **Milestone 21: Address Form**

- **Create Address Form Page:** Design and implement the frontend form for address input.
- **Store Address Data in State:** Store the inputted address data in a state.
- **Navigate to Address Form:** Clicking "Add Address" in the profile should navigate to the address form page.

---

### **Milestone 22: Add Address to User Collection**

- **Objective:** Implement a backend endpoint that will accept address data sent from the frontend address form.
- **Receive Address Data:** The backend should accept the address information (e.g., country, city, address1, address2, zip code, address type) from the frontend address form.
- **Update User Collection:** Add the received address to the address array inside the user collection in MongoDB.
- **Ensure Data Integrity:** Validate the address data before adding it to the user’s document to avoid invalid or incomplete entries.

---

### **Milestone 23: Place Order and Select Address**

- **Create Place Order Button in Cart:** Add a "Place Order" button inside the cart page that navigates to the select address page when clicked.
- **Create Select Address Page:** Implement a page that displays all available user addresses with an option to select one.
- **Backend Endpoint for Addresses:** Create a backend endpoint that returns all the addresses associated with the user.

---

### **Milestone 24: Display Order Summary and Place Order**

- **Objective:** Implement the order summary page to display the details of the user's order and allow them to place the order.
- **Display Products in Cart:** Show all the products the user is ordering, including their details such as name, quantity, and price.
- **Display Selected Address:** Show the selected delivery address that the user chose during the checkout process.
- **Display Total Cart Value:** Show the total value of the cart, including all items and any applicable taxes or discounts.
- **Place Order Button:** Add a "Place Order" button at the bottom of the page, allowing the user to confirm their order and proceed with the purchase.

---

### **Milestone 25: Order Creation and Storing Details**

- **Create Order Endpoint:** Develop an endpoint that receives product details, user information, and address details.
- **Retrieve User _id:** Using the user's email, fetch the _id of the user from the database.
- **Unique Order for Each Product:** Create a separate order for each product with the same address.
- **Store Order in MongoDB:** Use the order schema to store the order details in the MongoDB order collection.

---

### **Milestone 26: Retrieve User Orders**

- **Create Endpoint for User Orders:** Develop an endpoint that receives the user's email address.
- **Retrieve User _id:** Use the provided email to fetch the user's _id from the database.
- **Fetch All User Orders:** Using the user's _id, retrieve all the orders associated with that user.
- **Send Orders in Response:** Return all the retrieved orders in the response.

---

### **Milestone 27: My Orders Page**

- **Create My Orders Page:** Develop a new page for displaying user orders.
- **Send GET Request to Endpoint:** Send a GET request to the "my-orders" endpoint with the user's email to fetch their orders.
- **Retrieve User Orders:** Use the provided email to retrieve all orders associated with the user.
- **Display Orders on the Page:** Display all the retrieved user orders on the "my-orders" page.
- **Add My Orders to Navbar:** Add a link to the "my-orders" page in the navbar for easy navigation.

---

### **Milestone 28: Cancel Order Feature**

- **Add Cancel Order Button:** Implement a "Cancel Order" button on the "my-orders" page for each order.
- **Check Order Status:** Ensure the button is hidden if the order is already canceled.
- **Create Endpoint for Canceling Order:** Develop an endpoint that accepts the order ID.
- **Mark Order as Canceled:** Use the provided order ID to fetch the order and update its status to "canceled."
- **Save the Updated Order Status:** Save the updated order status in the database.

---

### **Milestone 29: PayPal Integration**

- **Create PayPal Account:** Set up a PayPal account and log into the PayPal Developer Dashboard.
- **Create Sandbox Account:** In the dashboard, create a sandbox account and save the UserID.
- **Get Client ID:** Copy and save the Client ID from the sandbox account.
- **Order Confirmation Page:** Add two payment options (COD and online payment) using radio buttons.
- **Display PayPal Buttons:** When "online payment" is selected, show PayPal payment buttons.
- **Next Milestone:** In the following milestone, implement functionality to use PayPal payment buttons.

---

### **Milestone 30: Implement Online Payment with PayPal**

- **Install PayPal SDK Package:** Install the react-paypal-js package using NPM.  
- **Set Up PayPalScriptProvider:** Use the PayPalScriptProvider component to load the PayPal SDK and display payment options.  
- **Use Client ID:** Provide your previously saved PayPal sandbox Client ID to the PayPalScriptProvider.  
- **Enable Online Payment Options:** Integrate PayPal payment methods such as credit or debit card on the order confirmation page.  
- **Test in Sandbox Mode:** Ensure the payment flow works correctly using the sandbox account.

---

