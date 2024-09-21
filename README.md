
# Shopping API

This project is a basic backend API developed using Flask and MySQL. It serves as a simple shopping application, where users can register, log in, add products to their cart, and simulate a purchase (without real payment integration). Admins can manage the products, including adding new products, updating stock, and deleting items.

This is **one of the first backend projects** I developed to familiarize myself with Flask and backend design principles. It is a simple, straightforward application focusing on the core concepts of backend development, authentication, and CRUD operations.

## Features

- **User Authentication & Authorization**: JWT (JSON Web Token) is used for secure authentication. There are separate endpoints for users and admins.
- **Shopping Functionality**: Users can add products to their cart, simulate a checkout process (without real payment integration), and view available products.
- **Admin Panel**: Admins can manage product inventories, add new products, update stock, and delete products.
- **MySQL Database**: The backend is connected to a MySQL database to store user, product, and order information.

## Technologies Used

- **Flask**: Web framework used for developing the backend.
- **MySQL**: The database for storing application data.
- **JWT**: Used for secure user authentication and authorization.
- **Docker**: The application is containerized using Docker, with Docker Compose managing the multi-container setup for the Flask application and MySQL database.

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/tarikalim/ShoppingAPI.git
cd ShoppingAPI
```

### 2. Create and Configure `.env` File

In the directory `ShoppingAPI\ShoppingAPI`, create a `.env` file with necessary variables (check example.env file) .

### 3. Update `docker-compose.yml`

In the root directory of the project, you will find a `docker-compose.yml` file. You need to update the MySQL credentials as required.

### 4. Build and Run the Application

After configuring the `.env` file and `docker-compose.yml`, navigate to the root directory and build/run the application with Docker Compose:

```bash
docker-compose up --build
```

This command will build the Flask app and start the MySQL database. The Flask app will be accessible at `http://localhost:5000`.



## Future Improvements

- **Payment Integration**: Real payment gateway integration for a complete shopping experience.
- **Frontend**: A frontend to provide a user-friendly interface for the shopping and admin functionalities.
