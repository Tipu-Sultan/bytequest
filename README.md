# API Routes Documentation

## Postman used for testing

#### http://127.0.0.1:8000/api/products

This document provides documentation for the API routes related to the `products` resource.

## List all products

### Request


### Description

Retrieves a list of all products.

### Response

- Status Code: 200 OK
- Content Type: application/json

# Example Response Body:

```json
[    {        "id": 1,        "name": "Product 1",        "description": "Description of Product 1",        "price": 10.99,        "quantity": 5,        "created_at": "2024-05-15T12:00:00Z",        "updated_at": "2024-05-15T12:00:00Z"    },    {        "id": 2,        "name": "Product 2",        "description": "Description of Product 2",        "price": 15.99,        "quantity": 10,        "created_at": "2024-05-15T12:00:00Z",        "updated_at": "2024-05-15T12:00:00Z"    }]


POST /products

{
    "id": 1,
    "name": "Jean Product",
    "description": "Description of New Product",
    "price": 20.99,
    "quantity": 8,
    "created_at": "2024-05-15T12:00:00Z",
    "updated_at": "2024-05-15T12:00:00Z"
}


GET /products/{id}


{
    "id": 1,
    "name": "jeans Product ",
    "description": "Description of jeans ",
    "price": 10.99,
    "quantity": 5,
    "created_at": "2024-05-15T12:00:00Z",
    "updated_at": "2024-05-15T12:00:00Z"
}


PUT /products/{id}
{
    "id": 1,
    "name": "Updated Product",
    "description": "Updated Description of jeans",
    "price": 15.99,
    "quantity": 7,
    "created_at": "2024-05-15T12:00:00Z",
    "updated_at": "2024-05-15T12:00:00Z"
}


DELETE /products/{id}
{
    "message": "Product deleted successfully"
}