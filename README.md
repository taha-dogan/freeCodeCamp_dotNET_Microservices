## Web API for Managing Items

This repository contains a simple Web API for managing items. The API allows you to perform basic CRUD (Create, Read, Update, Delete) operations on items.

### Endpoints

- **GET /items**: Retrieves all items.
- **GET /items/{id}**: Retrieves a specific item by its ID.
- **POST /items**: Creates a new item.
- **PUT /items/{id}**: Updates an existing item.
- **DELETE /items/{id}**: Deletes an item.

### Usage

- **GET /items**: 
  - Response: Array of item objects.
- **GET /items/{id}**: 
  - Parameters: `id` (Guid) - ID of the item to retrieve.
  - Response: Single item object.
- **POST /items**: 
  - Body: JSON object containing item details.
  - Response: Created item object with its ID.
- **PUT /items/{id}**: 
  - Parameters: `id` (Guid) - ID of the item to update.
  - Body: JSON object containing updated item details.
  - Response: No content.
- **DELETE /items/{id}**: 
  - Parameters: `id` (Guid) - ID of the item to delete.
  - Response: No content.

### Data Formats

- **ItemDto**: Represents an item.
  - Properties: ID (Guid), Name (string), Description (string), Price (decimal), CreatedDate (DateTimeOffset).
- **CreateItemDto**: Data transfer object for creating a new item.
  - Properties: Name (string), Description (string), Price (decimal).
- **UpdateItemDto**: Data transfer object for updating an existing item.
  - Properties: Name (string), Description (string), Price (decimal).

### Technologies Used

- C#
- ASP.NET Core
- Microsoft.AspNetCore.Mvc

### How to Run

1. Clone this repository.
2. Open the solution in Visual Studio or your preferred C# IDE.
3. Build and run the solution.
4. Use your favorite API testing tool (e.g., Postman) to interact with the API endpoints.

### Contributors

- taha-dogan
