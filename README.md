# API-DOCUMENTATION

## Login
- **URL**: https://test.ludocorner.xyz/api/login
- **Method**: POST
- **Headers**: Content-Type: application/json
- **Body Credentials**: 
  - email: test.user@gmail.com
  - password: 12345678

Description: Use this endpoint to login and obtain a token for authentication. The token will be used for all subsequent API calls.

## Show Product
- **URL**: https://test.ludocorner.xyz/api/product/view_product
- **Method**: GET
- **Headers**: 
  - Authorization: Bearer {token}
  - Content-Type: application/json
- **Body Credentials**: NULL

Description: This endpoint retrieves the product list in a paginated format. Each page contains 10 products. Scroll the page to view more products.

## Show Single Product
- **URL**: https://test.ludocorner.xyz/api/product/view_single_product/{product_id}
- **Method**: GET
- **Headers**: 
  - Authorization: Bearer {token}
  - Content-Type: application/json
- **Body Credentials**: NULL

Description: This endpoint retrieves the details of a single product, including an image. Replace `{product_id}` in the URL with the actual ID of the product.

## Add Cart
- **URL**: https://test.ludocorner.xyz/api/cart/add_cart
- **Method**: POST
- **Headers**: 
  - Authorization: Bearer {token}
  - Content-Type: application/json
- **Body Credentials**: 
  - product_id: {product_id}

Description: This endpoint adds a product to the user's cart. Provide the `product_id` in the request body to add the corresponding product.

## Show Cart
- **URL**: https://test.ludocorner.xyz/api/cart/view_cart
- **Method**: GET
- **Headers**: 
  - Authorization: Bearer {token}
  - Content-Type: application/json
- **Body Credentials**: NULL

Description: This endpoint retrieves the items in the user's cart. Authenticate using the token and click on the cart icon to view the cart items.
# API Testing Instructions

## Technology Used
- Postman: API testing tool used for sending requests and validating responses.
- Newman: Command-line companion for Postman that allows for running collections and generating reports.

## Prerequisites
- JDK: Java Development Kit is required for running Postman.
- Node.js: JavaScript runtime environment required for installing and running Newman.

## Newman and HTML Report Installation Process

### Step 1: Install Newman
To install Newman, open a terminal or command prompt and run the following command:

### Step 2: Install Newman HTML Report
To install the Newman HTML report library, run the following command:

### Step 3: Generate HTML Reports
After running Newman, you can generate an HTML report using the following command:
Replace `<collection_file_path>` with the path to your Postman collection file.

The HTML report will be generated in the `newman` folder in your current directory.

### Newman Report Summary:



