# Flask Web Application

This is a simple Flask-based web application that allows users to register, log in, and view products. The application interacts with several microservices to handle user authentication and product retrieval.

## Features

- **User Registration**: Users can register by providing a username and password.
- **User Login**: Registered users can log in to access the products page.
- **View Products**: After logging in, users can view a list of products retrieved from a microservice.

## Requirements

- Python 3.x
- Flask
- Requests
- Python-dotenv
- Flask-CORS

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/stwins60/ecommerce-platform.git
   cd ecommerce-platform/frontend
   ```
2.  Create a virtual environment:
    - For Windows:
        ```bash
        python -m venv venv
        venv\Scripts\activate
        ```
    - For macOS/Linux:
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```

3.  **Install the dependencies:**
    -  For Windows:
        ```bash
        pip install -r requirements.txt
        ```
    -  For macOS/Linux:
          ```bash
            pip3 install -r requirements.txt
            ```
4.  **Set the environment variables:**
    create a `.env` file in the `frontend` directory and add the following variables:
    ```plaintext
    REGISTER_URL=<your_register_url>
    LOGIN_URL=<your_login_url>
    PRODUCTS_URL=<your_products_url>
    ```
5.  **Run the application:**
    -  For Windows:
        ```bash
        set FLASK_APP=app.py
        flask run
        ```
    -  For macOS/Linux:
        ```bash
        export FLASK_APP=app.py
        flask run
        ```
6.  **Access the application:**
    Open a web browser and go to `http://127.0.0.1:5000/` to view the application.