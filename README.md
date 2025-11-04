# E-commerce API

This is a boilerplate for a basic e-commerce API built with Python and FastAPI.

## Features

* User authentication and authorization
* Product and category management
* Shopping cart and order processing
* Payment integration (mock)

## Project Structure

*   **models/**: Defines the database tables (User, Role, Category, Product, Cart, Order, Payment).
*   **repositories/**: Provides low-level CRUD (Create, Read, Update, Delete) operations for the database.
*   **services/**: Contains the core business logic, such as checkout, pricing, and stock validation.
*   **controllers/**: Includes route handlers that map HTTP endpoints to specific functions.
*   **routes/**: Assembles the application's routers using `include_router`.
*   **schemas/**: Uses Pydantic for data validation and serialization (input/output).
*   **middlewares/**: Implements authentication, validation, and request tracking.
*   **configs/**: Manages database connections, environment variables, and constants.
*   **utils/**: Provides helper functions, including JWT handling and standardized response formats.
*   **core/**: Includes utilities for logging, caching, and security.
*   **tests/**: Contains isolated tests for each domain.

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/e-commerce-api.git
    cd e-commerce-api
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv .venv
    source .venv/bin/activate
    ```

3.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Run the development server:**
    ```bash
    uvicorn src.server:app --reload
    ```

2.  **Access the API documentation:**
    Open your browser and navigate to `http://127.0.0.1:8000/docs` to view the interactive API documentation.