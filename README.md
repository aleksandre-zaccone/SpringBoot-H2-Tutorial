# Product Management API using Spring Boot

This repository contains a simple Product Management API developed using Spring Boot. The API allows you to manage products, including adding, updating, retrieving, and deleting products.

## Getting Started

To run this project locally using Gradle and IntelliJ IDEA, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/product-management-api.git
   
2. Open IntelliJ IDEA.

* From the main menu, select File > Open and navigate to the project directory.
* In IntelliJ IDEA, import the project as a Gradle project
* Select build.gradle in the root of the project.
* Click Open.
* Once the project is imported, locate and run the ProductManagementApiApplication class. This will start the Spring Boot application.

The API will be accessible at http://localhost:8080/api/products.

# Endpoints
The following API endpoints are available:

### GET All Products:
* Method: GET
* URL: http://localhost:8080/api/products

### GET Product by ID:
* Method: GET 
* URL: http://localhost:8080/api/products/{id}
* Example: http://localhost:8080/api/products/1

### GET Products by Name (Search):
* Method: GET
* URL: http://localhost:8080/api/products/search?name={name}
* Example: http://localhost:8080/api/products/search?name=Google%20Fold%20Phone

### POST Add Product:
* Method: POST 
* URL: http://localhost:8080/api/products
* Headers: Content-Type: application/json 
* Body (raw JSON):
```json
{
  "name": "Google Fold Phone",
  "price": 1499.99
}
```

### PUT Update Product by ID:
* Method: PUT 
* URL: http://localhost:8080/api/products/{id}
* Example: http://localhost:8080/api/products/1
* Headers: Content-Type: application/json 
* Body (raw JSON):
```json
{ "name": "Updated Google Fold Phone", "price": 1599.99 }
```

### DELETE Product by ID:
* Method: DELETE 
* URL: http://localhost:8080/api/products/{id}
* Example: http://localhost:8080/api/products/1

# To use Postman:
* Open Postman. 
* Select the appropriate HTTP method (GET, POST, PUT, DELETE). 
* Enter the endpoint URL. 
* If required, add headers (such as Content-Type: application/json) based on the request. 
* Add the request body (for POST and PUT requests) in JSON format. 
* Click the "Send" button to make the request.

You can customize the examples above based on your specific use case and the actual data you want to send or receive.


# Contributing
Contributions are welcome! Feel free to open issues or submit pull requests for improvements.
