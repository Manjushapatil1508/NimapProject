# NimapProject
using Spring Boot, Hibernate, and JPA. It manages Categories and Products with a one-to-many relationship and supports CRUD (Create, Read, Update, Delete) operations. The project includes server-side pagination for efficient data handling and leverages annotation-based configuration.

Features
Spring Boot Framework: Simplifies the setup and development of the project.
RESTful API: Exposes endpoints for managing categories and products.
Hibernate and JPA: Manages database interactions and relationships between entities.
Annotation-based Configuration: All configurations are annotation-driven, avoiding the use of XML.
One-to-Many Relationship: Implements a relationship between Category and Product entities.
Server-side Pagination: Supports paginated fetching of data for better performance.


Technologies Used
Java 11+: Programming language used for building the application.
Spring Boot: Framework used to create stand-alone, production-ready Spring applications.
Spring Data JPA: Simplifies the database layer implementation.
Hibernate: ORM (Object-Relational Mapping) framework for mapping Java objects to relational database tables.
MySQL: Relational database used for data persistence.
Maven: Build tool used for project management and dependency management.
Getting Started


Prerequisites
Java 11 or newer installed on your machine.
MySQL database set up and running.
Maven installed for building and running the project.

API Endpoints
Category Endpoints
GET /api/categories?page={page}: Retrieve paginated list of categories.
POST /api/categories: Create a new category.
GET /api/categories/{id}: Retrieve a category by its ID.
PUT /api/categories/{id}: Update an existing category by its ID.
DELETE /api/categories/{id}: Delete a category by its ID.


Product Endpoints
GET /api/products?page={page}: Retrieve paginated list of products.
POST /api/products: Create a new product.
GET /api/products/{id}: Retrieve a product by its ID.
PUT /api/products/{id}: Update an existing product by its ID.
DELETE /api/products/{id}: Delete a product by its ID.


Project Structure
entity/: Contains the JPA entity classes Category and Product.
repository/: Contains the repository interfaces for database operations.
service/: Contains service interfaces and their implementations for business logic.
controller/: Contains REST controllers to handle HTTP requests.
application.properties: Configuration file for database and JPA settings.
Database Model
Category: Represents a product category with a one-to-many relationship to Product.
Product: Represents a product with a reference to its Category.
