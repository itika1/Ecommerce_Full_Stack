# Product Category Ecommerce Application

## Overview
This is a full-stack eCommerce application designed to manage products and categories. The backend is built using Java and Spring Boot, and the frontend is developed with a web framework of your choice. The application supports CRUD operations for products and categories, user authentication, and various other eCommerce functionalities.

## Features
- User registration and authentication
- CRUD operations for products and categories
- Product search and filtering
- Shopping cart functionality
- Order management
- Admin panel for managing products and categories

## Technologies Used
### Backend
- Java
- Spring Boot
- Spring Data JPA
- Maven
- MySQL (or any other relational database)

### Frontend
- React

### Others
- Spring Security
- Thymeleaf (if using server-side rendering)
- Lombok (for reducing boilerplate code)
- JUnit and Mockito (for testing)
- Docker (for containerization)

## Installation

### Prerequisites
- Java 11 or higher
- Maven
- MySQL (or any other relational database)
- Node.js and npm (if using a JavaScript framework for frontend)
- Docker (optional, for containerization)

### Backend Setup
1. Clone the repository:
    ```sh
    git clone https://github.com/itika1/ecommerce-app.git
    cd ecommerce-app
    ```

2. Update the database configuration in `application.properties`:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce
    spring.datasource.username=root
    spring.datasource.password=yourpassword
    spring.jpa.hibernate.ddl-auto=update
    ```

3. Build the project:
    ```sh
    mvn clean install
    ```

4. Run the application:
    ```sh
    mvn spring-boot:run
    ```

### Frontend Setup
1. Navigate to the frontend directory:
    ```sh
    cd frontend
    ```

2. Install dependencies:
    ```sh
    npm install
    ```

3. Start the development server:
    ```sh
    npm start
    ```

## API Endpoints
### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login a user

### Products
- `GET /api/products` - Get all products
- `GET /api/products/{id}` - Get product by ID
- `POST /api/products` - Create a new product (Admin only)
- `PUT /api/products/{id}` - Update a product (Admin only)
- `DELETE /api/products/{id}` - Delete a product (Admin only)

### Categories
- `GET /api/categories` - Get all categories
- `GET /api/categories/{id}` - Get category by ID
- `POST /api/categories` - Create a new category (Admin only)
- `PUT /api/categories/{id}` - Update a category (Admin only)
- `DELETE /api/categories/{id}` - Delete a category (Admin only)

### Orders
- `GET /api/orders` - Get all orders (Admin only)
- `GET /api/orders/{id}` - Get order by ID (Admin only)
- `POST /api/orders` - Create a new order
- `PUT /api/orders/{id}` - Update an order (Admin only)
- `DELETE /api/orders/{id}` - Delete an order (Admin only)

## Running Tests
1. Run unit tests:
    ```sh
    mvn test
    ```

2. Run integration tests:
    ```sh
    mvn verify
    ```

## Docker Support
1. Build Docker images:
    ```sh
    docker-compose build
    ```

2. Run containers:
    ```sh
    docker-compose up
    ```

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

## Contact
Itika Sarkar - [itikaitzme@gmail.com](mailto:itikaitzme@gmail.com)

Project Link: [https://github.com/itika1/ecommerce-app](https://github.com/itika1/ecommerce-app)
