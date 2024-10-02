# API Testing Project

## Overview

This project contains automated tests for various API endpoints using Java, RestAssured, and Mockoon for mocking API responses.

## Setting Up Mockoon

1. **Download and Install Mockoon**:
    - Visit [Mockoon's website](https://mockoon.com/download) and download the appropriate version for your operating system.
    - Install Mockoon.

2. **Import the Mockoon Environment**:
    - Open Mockoon.
    - Click on the "Import" button and select the provided `BookStore.json` file from this project, can be found in the config package.
    - This environment contains all the mock APIs configured for testing.

3. **Start the Mock Server**:
    - Select the imported environment in Mockoon.
    - Click the "Play" button to start the mock server.
    - Make sure the server is running on `http://localhost:3001`.

## Run the test

- clone the repo
- Run the test by run
    ```bash
   mvn test

## Postman Collection

To facilitate manual testing of the APIs, a Postman collection is provided. This collection is located in the `/tests/integration` directory as `API_Test_Collection.json`. 
