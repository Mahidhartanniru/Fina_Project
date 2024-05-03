## Project Overview

### Introduction

This project showcases a seamless integration of FastAPI framework with SQLite database, enabling a robust CRUD (Create, Read, Update, Delete) API. The API facilitates the management of customers, items, and orders effortlessly.

### Key Features

- Perform CRUD operations on customers, items, and orders.
- Create, read, update, and delete customers.
- Create, read, update, and delete items.
- Create and read orders.

### Prerequisites

Ensure the following prerequisites are met before proceeding:

- Python 3.7 or later installed on your system.
- Virtual environment set up.
- Dependencies installed.

### Execution Steps

Follow these steps to execute the project:

1. **Create a Virtual Environment:**
    - Execute `python -m venv venv`.

2. **Activate the Virtual Environment:**
    - For Windows: `venv\Scripts\activate`.
    - For Unix or MacOS: `source venv/bin/activate`.

3. **Install Dependencies:**
    - Run `pip install fastapi`.
    - Run `pip install uvicorn`.
    - Run `pip install pydantic`.

4. **Initialize the SQLite Database:**
    - Execute `python db_init.py`.
    - This script will create necessary tables and populate them with sample data from `example_orders.json`.

5. **Run the FastAPI Server:**
    - Execute `uvicorn main:app --reload`.
    - The server will start running on `http://127.0.0.1:8000`.

6. **Access the API Documentation:**
    - Open your web browser and navigate to `http://127.0.0.1:8000/docs`.
    - Here, you can explore and interact with the API endpoints using the Swagger UI.

### API Endpoints

#### Customers:
- **POST /customers/:** Create customer.
- **GET /customers/{cust_id}:** Read Customer.
- **PUT /customers/{cust_id}:** Update Customer.
- **DELETE /customers/{cust_id}:** Delete Customer.

#### Items:
- **POST /items/:** Create item.
- **GET /items/{item_id}:** Read item.
- **PUT /items/{item_id}:** Update item.
- **DELETE /items/{item_id}:** Delete item.

#### Orders:
- **POST /orders/:** Create Order.
- **GET /orders/{order_id}:** Read Order.
- **PUT /orders/{order_id}:** Update Order.
- **DELETE /orders/{order_id}:** Delete Order.
