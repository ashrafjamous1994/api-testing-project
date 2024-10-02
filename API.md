# API Endpoints

# User Registration
- **Endpoint:** `POST /users/register`
- **Request:**
  ```json
  {
    "email": "string"
    "password": "string",
  }
- **Response (Success):**
  ```json
  {
  "message": "User registered successfully.",
  "userId": "string"
  }
- **Response (Error):**
  ```json
  {
  "error": "string" // e.g. email already exists.
  }

# User Login
- **Endpoint:** `POST /users/login`
- **Request:**
  ```json
  {
  "email": "string",  
  "password": "string"   
  }
- **Response (Success):**
  ```json
  {
  "message": "Login successful.",  
  }
  - **Response (Error):**
    ```json
    {
    "error": "string" // e.g., Invalid credentials.
    }

# Search Books
- **Endpoint:** `GET /books?search=query`
- **Response (Success):**
  ```json
  {
  "books": [
    {
      "id": "string",    
      "title": "string",  
      "price": "number"   
    }
  ]
  }
- **Response (Error):**
  ```json
  {
  "error": "string" // e.g., No books found or Query parameter is required
  }

# Add to Cart
- **Endpoint:** `POST /users/{userId}/cart`
- **Request:**
  ```json
  {
  "bookId": "string",
  }
  
- **Response (Success):**
  ```json
  {
  "message": "Book added to cart."
  }
- **Response (Error):**
  ```json
  {
  "error": "string" // e.g., Book not found.
  }

# Checkout
- **Endpoint:** `POST /users/{userId}/checkout`
- **Request:**
  ```json
  {
  "paymentMethod": "string"
  }

- **Response (Success):**
  ```json
  {
  "message": "Checkout successful.",
  }
- **Response (Error):**
  ```json
  {
   "error": "string" // e.g., Invalid payment method.
  }
  
