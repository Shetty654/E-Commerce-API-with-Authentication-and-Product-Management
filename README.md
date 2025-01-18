# E-Commerce API with Authentication and Product Management  

## Overview  
This project is a RESTful API for managing e-commerce operations, developed using Spring Boot. It includes functionality for category and product management, keyword-based search, and user authentication. The application is designed to cater to both public users and administrators.  

## Features  
- **Public APIs**:  
  - View and search products by keyword  
  - View product details and associated images  
  - Browse categories and their products  
  - Sort categories for easier navigation  

- **Admin APIs**:  
  - Manage categories (create, update, delete)  
  - Add, update, and delete products in categories  

- **Authentication**:  
  - User signup and login  

## API Endpoints  

### Public Endpoints  
1. **Get All Categories**  
   `GET /api/public/categories`  
2. **Sort Categories**  
   `GET /api/public/categories?sortBy=categoryName&orderBy=asc`  
3. **Get Specific Category**  
   `GET /api/public/categories/{id}`  
4. **Get Products in a Category**  
   `GET /api/public/categories/{id}/products`  
5. **Get Product Details**  
   `GET /api/public/products/{id}`  
6. **Get Product Image**  
   `GET /api/public/products/{id}/image`  
7. **Search Products by Keyword**  
   `GET /api/public/products/keyword/{keyword}`  

### Admin Endpoints  
1. **Manage a Category**  
   `GET, POST, PUT, DELETE /api/admin/categories/{id}`  
2. **Add Product to a Category**  
   `POST /api/admin/categories/{id}/product`  
3. **Manage a Product**  
   `GET, POST, PUT, DELETE /api/admin/products/{id}`  

### Authentication Endpoints  
1. **User Sign-in**  
   `POST /api/auth/signin`  
2. **User Sign-up**  
   `POST /api/auth/signup`  

## Technologies Used  
- **Backend**: Spring Boot, Java  
- **Database**: H2/MySQL (configurable)  
- **Build Tool**: Maven  

## Getting Started  

### Prerequisites  
- Java 11 or higher  
- Maven 3.6+  
- An IDE like IntelliJ IDEA or Eclipse  

### Steps to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/ecommerce-api.git
