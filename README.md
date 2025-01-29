# **E-commerce Product API**

## **Project Overview**
Implementing an E-commerce Product API using Django and Django REST Framework. This API will serve as the backend for managing products on an e-commerce platform, allowing users to create, update, delete, and view products. You will build and deploy a fully functional API, mimicking the real-world responsibilities of a backend developer in the e-commerce space, focusing on product management, user authentication, and search functionality.

## **Functional Requirements**

### **Product Management (CRUD):**
- Ability to Create, Read, Update, and Delete (CRUD) products.
- Each product have the following attributes:
  - Name
  - Description
  - Price
  - Category
  - Stock Quantity
  - Image URL
  - Created Date
- Validation for required fields like Price, Name, and Stock Quantity.
- Stock Quantity is automatically reduced when an order is placed.
- 
### Users Management (CRUD):
- CRUD operations for users who will manage the products.
- Username, Email, and Password.
- Only authenticated users will be able to manage products (i.e., create, update, delete).

### Product Search:
- Endpoint to search for products by Name or Category.
- Pagination for search results to improve performance when there are many products.

### **Product View:**
- Endpoint to retrieve a list of products or view individual product details by Product ID.
- Optional filter for users to view products by:
  - Category
  - Price Range
  - Stock Availability
- Description, Price, Category, Stock Quantity, and Image URL.

## **Technical Requirements**

### **Database:**
- Django ORM to interact with the database.
- Models for Products and Users.
- Product organization (e.g., Electronics, Clothing, etc.).

### **Authentication:**
- User authentication using Django’s built-in authentication system.
- Authenticated can perform CRUD operations on products.
- Token-based authentication (JWT) to secure the API further.

### **API Design:**
- Django Rest Framework (DRF) to design and expose API endpoints.
- RESTful principles using appropriate HTTP methods (GET, POST, PUT, DELETE).
- Proper error handling, returning appropriate HTTP status codes for various actions (e.g., 404 for not found, 400 for bad request).

### **Deployment:**
- Deployment of the API on Heroku
- Deployed API is accessible, stable, and secure.

### Pagination and Filtering:
- Pagination for product listing and search endpoints to handle large datasets efficiently.
- Filtering options for:
  - Category
  - Price Range
  - Stock Availability
