Play Catalog Service API
This is a simple RESTful API for managing items in a catalog. It provides endpoints to perform CRUD operations on items.

Endpoints
GET /items

Retrieves a list of all items in the catalog.
GET /items/{id}

Retrieves the details of a specific item by its unique identifier.
POST /items

Creates a new item in the catalog.
Request Body:
json
Copy code
{
  "name": "string",
  "description": "string",
  "price": "decimal"
}
Constraints:
name (required): Name of the item.
description: Description of the item.
price (range: 0-1000): Price of the item.
PUT /items/{id}

Updates an existing item in the catalog.
Request Body:
json
Copy code
{
  "name": "string",
  "description": "string",
  "price": "decimal"
}
Constraints:
name (required): New name of the item.
description: New description of the item.
price (range: 0-1000): New price of the item.
DELETE /items/{id}

Deletes an item from the catalog.
Data Transfer Objects (DTOs)
ItemDto

Represents the data structure of an item.
Fields:
Id: Unique identifier of the item.
Name: Name of the item.
Description: Description of the item.
Price: Price of the item.
CreatedDate: Date and time when the item was created.
CreateItemDto

Represents the data structure for creating a new item.
Fields:
Name (required): Name of the item.
Description: Description of the item.
Price (range: 0-1000): Price of the item.
UpdateItemDto

Represents the data structure for updating an existing item.
Fields:
Name (required): New name of the item.
Description: New description of the item.
Price (range: 0-1000): New price of the item.
Usage
Clone the repository.
Navigate to the project directory.
Build and run the application.
Access the API endpoints using a tool like Postman or any HTTP client.
