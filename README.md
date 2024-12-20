# REST API for Product Management

## Description
This project implements a simple REST API to manage products using Python and Flask. It supports creating and retrieving product information.

## Setup Instructions
1. Clone the repository:
    ```bash
    git clone https://github.com/Maxwell619/Question-2
    cd Question-2
    ```

2. Install dependencies:
    pip install flask requests
  

3. Run the API server:
    python app.py
    

4. Test the API:
   - Use the client script:
     python client.py
    
 

## API Endpoints
### POST /products
- **Description**: Create a new product.
- **Request JSON Format**:
    ```json
    {
        "name": "Product Name",
        "description": "Product Description",
        "price": 10.5
    }
    ```
- **Response**:
    - `201 Created`: Returns the created product.
    - `400 Bad Request`: For invalid input.

### GET /products
- **Description**: Retrieve all products.
- **Response**:
    - `200 OK`: Returns a list of products.

---

## Client Script
The `client.py` script demonstrates how to interact with the API:
- Adds products using `/products`.
- Retrieves the list of all products.
