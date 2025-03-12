# Ecommerce_Follow_Along
Follow along project for sem 2.


**Milestone 1**: *Project Overview*  

In todays live session our mentor introduced us to overall structure of MERN Stack.
He taught us the foundational steps to set up the environment for future milestones.
We created a new repository for our follow along project.


**Milestone 2**

Organize Your Project: Separate your files into two main folders—one for the frontend and one for the backend.
Set Up React Frontend: Create a React app to build the user interface for your project.
Set Up Node.js Backend: Build a basic Node.js server to prepare for adding APIs later.
Configure Tailwind CSS: Add Tailwind CSS for easy, modern styling that works well on any screen size.
Build Login Page: Design and develop the first page of your e-commerce app, focusing on both its look and functionality.


**Milestone 3**

Set up dedicated folders for organizing backend code effectively.
Initialize and configure a Node.js server to handle API requests.
Connect your application to MongoDB to store and manage data.
Implement basic error handling to ensure your server runs smoothly.
Update the README file to document your progress.


**Milestone 4**

Created a User Model: Our mentor explained how a MODEL in MVC architecture works and how it interacts with database.
Created a User Controller: We got to know the purpose of a controller in MVC.
Enable and Configure Multer: In the live session mentor told us what is a multer and what is it used for and how it can be configured to handle file uploads.


**Milestone 5**

Create a Sign-Up page: Users enter details (Name, Email, Password) to register.
Implement form validation: Ensure correct data format (e.g., valid email and secure password).
Build frontend: Use HTML and CSS for the design.
Document progress: Update the README file with what I've accomplished.


**Milestone 6**

Encrypt Password with bcrypt..
Use bcrypt to hash the user's password during signup, ensuring it is stored securely and not in plain text.
Save Hashed Password in Database..
Only store the hashed version of the password in the database. Never save the plain text password.
Store Complete User Data..
Save the user's other information (e.g., name, email) along with the hashed password securely.
Login with Hashed Password..
During login, compare the entered password with the hashed password in the database using bcrypt for verification.

**Milestone 7** 

Learning Goals:-
Validate user login credentials.
Securely compare encrypted passwords.

Why Encrypt Passwords..?
Security: Protects data if the database is breached.
Privacy: Prevents storing plain-text passwords.
Compliance: Follows security standards (e.g., GDPR, PCI-DSS).
Prevention: Hardens password theft with hashing.

Login Authentication Process:-
User enters credentials (email/username & password).
Check if the user exists in the database.
Use bcrypt to compare hashed passwords.

Steps to Implement:-
Create login endpoint for credentials.
Fetch user data from the database.
Hash input password and compare with stored hash.


**Milestone 8**

Learning Goals:-
Create a card component for products.
Display product cards on the homepage.

Why Create Card Components..?
Showcase products clearly and visually.
Reusable design across pages.
Improves user experience and interaction.
Keeps the homepage organized.

Displaying Multiple Product Cards:-
Design a dynamic card component using props.
Use array mapping to render multiple cards.
Pass product info (name, price, image) to each card.
Ensure consistent layout for all cards.

Steps:-
Create a reusable card component.
Set up a grid or flexbox layout for the homepage.


**Milestone 9**

In this milestone we have created
Create the form for products
This form will take multiple product images images as input


**Milestone 10**

In this milestone we have learnt how to write product schema.

Learnt how to create an end point to validate and store product details in mongodb.


**Milestone 11**

In this milestone we have learnt how to"

Write an endpoint that will send data from extract and send data from mongodb.

Receive data at frontend -How to display that data dynamically using product card created earlier.


**Milestone 12**

In this milestone we have learnt how to write an endpoint that will send data by filtering with my mail and send data from mongodb.

Also how to receive data at frontend.

How to display that data dynamically using product card created earlier.


**Milestone 13**

Goal: Learn how to update existing data in MongoDB and edit product details.  
Backend: Write an endpoint to receive new data and update existing data in MongoDB.  
Frontend: Add an edit button on product cards to trigger the edit form.  
Form: Autofill the form with previous data, allowing the user to edit and save.  
Outcome: Understand the process of performing update operations in MongoDB.  


**Milestone 14**

Write an endpoint that will Delete the data form MongoDB using ID.  
In frontend we will add an delete button to the product card. When click on delete button we will send the product id to server endpoint.


**Milestone 15**

Build a Nav component with links (Home, My-products, Add product, Cart).  
Make it responsive and reusable across pages.  
Outcome: Easy navigation between pages in a React app.  


**Milestone 16**

Create a new page to showcase the product details.  
Add functionality for selecting quantity.  
Implement an "Add to Cart" button.  


**Milestone 17**

Write the cart schema to store products.  
Write an endpoint to store receive and store product details in cart.  


**Milestone 18**

Create an Backend endpoint for cart page.  
Write and endpoint to get products inside cart for user.  

**Milestone 19**

1. Create Cart Frontend Page:

- Display Products: Fetch and display all the products that the user has added to the cart from an existing backend endpoint (from Milestone 18).
- Product Information: For each product, show the product name, price, quantity, and total price (quantity multiplied by price).

Quantity Adjustment: For each product, include two buttons:

- A "+" button to increase the quantity of the product.
- A "-" button to decrease the quantity of the product.

Update Total: Ensure the total price updates accordingly when the quantity changes.

2. Create Backend Endpoints for Quantity Update:

- Increase Quantity Endpoint: This endpoint should accept a request to increase the quantity of a specific product in the cart.
- Decrease Quantity Endpoint: This endpoint should accept a request to decrease the quantity of a specific product in the cart.

Business Logic: Ensure that the quantity cannot go below 1 (or other logical limits depending on the business rules). Additionally, the backend should handle updating the cart’s total cost as the quantity changes.

3. Connect Frontend to Backend:

- Frontend Communication: Use AJAX or Fetch API to send requests to the backend when a user clicks the "+" or "-" buttons for a product.

- Dynamic Updates: After receiving a response from the backend, dynamically update the UI to reflect the new quantity and updated total price for the product in the cart.

4. Test Functionality
- Verify Updates: Ensure that the frontend correctly reflects changes in quantity and price when users click the + and - buttons.

- Check Backend: Test the backend endpoints to confirm that they correctly update the cart and handle errors 