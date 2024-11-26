# **Nimap Machine Test - CRUD Application**

## **Features**

1. **Product Management**:

   - Create, Read, Update, and Delete products.
   - Pagination support for fetching products.
   - Association of products with categories.

2. **Category Management**:

   - Create, Read, Update, and Delete categories.
   - Pagination support for fetching categories.
   - Categories are independent and not affected by products.

3. **Error Handling**:

   - Custom exception handling using a `GlobalExceptionHandler`.
   - Clear error messages for invalid or missing resources.

4. **Database**:
   - MySQL database integration for persistent storage.
   - JPA and Hibernate for ORM.

---

## **Technologies Used**

1. **Backend**:

   - Java 17
   - Spring Boot 3
   - Spring Data JPA
   - Spring Web

2. **Database**:

   - MySQL 8

3. **Build Tools**:

   - Maven

4. **Testing**:
   - Postman (for manual API testing)



## **API Documentation**

### **Categories**

| Method | Endpoint                 | Description                    | Request Body                |
| ------ | ------------------------ | ------------------------------ | --------------------------- |
| POST   | `/api/categories`        | Create a new category          | `{ "name": "Electronics" }` |
| GET    | `/api/categories?page=0` | Get all categories (paginated) | N/A                         |
| GET    | `/api/categories/{id}`   | Get category by ID             | N/A                         |
| PUT    | `/api/categories/{id}`   | Update category by ID          | `{ "name": "Gadgets" }`     |
| DELETE | `/api/categories/{id}`   | Delete category by ID          | N/A                         |

---

### **Products**

| Method | Endpoint               | Description                  | Request Body                                                             |
| ------ | ---------------------- | ---------------------------- | ------------------------------------------------------------------------ |
| POST   | `/api/products`        | Create a new product         | `{ "name": "Laptop", "price": 1500, "category": { "catId": 1 } }`        |
| GET    | `/api/products?page=0` | Get all products (paginated) | N/A                                                                      |
| GET    | `/api/products/{id}`   | Get product by ID            | N/A                                                                      |
| PUT    | `/api/products/{id}`   | Update product by ID         | `{ "name": "Gaming Laptop", "price": 2000, "category": { "catId": 2 } }` |
| DELETE | `/api/products/{id}`   | Delete product by ID         | N/A                                                                      |

## **Contact**

- **Name**: Prajwal Atul Patil
- **Email**: pp28032001@gmail.com

---
"# Nimap-Machine-Test-" 
