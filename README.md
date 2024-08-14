**Postman Collection and Environment for Petshop API**

**Description**

This repository contains a Postman collection and environment designed for comprehensive testing of the Petshop API. The collection includes various endpoints to manage pets in the system, such as creating, updating, and deleting pet records. Both positive and negative test cases have been created to ensure the correct functionality of the API and to handle potential errors.

**Repository Contents**

Postman Collection (petshop-api-collection.json): Includes requests to interact with the Petshop API. The covered endpoints are:

Create Pet: Tests the functionality to add a new pet to the system.
Get Pet: Verifies that the information of a specific pet can be retrieved using its ID.
Update Pet: Evaluates the ability to modify the data of an existing pet.
Delete Pet: Ensures that a pet can be correctly deleted from the system.
List Pets: Validates the retrieval of a list of all registered pets.

Postman Environment (petshop-api-environment.json): Configures the necessary variables for running the tests. It includes:

Base URL: The base URL for the Petshop API.
Pet ID: A dynamic variable that stores the pet ID generated during the tests.

**Test Cases**

Positive Cases: Verifies that the system performs the expected operations correctly when provided with valid data.
Negative Cases: Assesses how the system handles unexpected situations or invalid data, ensuring that it responds appropriately to errors and exceptions.

**Features**

Automation with Newman: The collection is designed to be run automatically with Newman, allowing for integration into CI/CD pipelines and facilitating regular automated testing.
Screenshots: Screenshots are captured both on success and failure to assist in documentation and error reporting.

**Usage Instructions**

Import the collection and environment into Postman:

Open Postman and select "Import."
Upload the files petshop-api-collection.json and petshop-api-environment.json.

**Configure the Environment:**

Select the "Petshop API" environment in the Postman interface.
Run Tests with Newman:

Install Newman if you haven't already: npm install -g newman.
Run the tests using the following command:
bash
Copiar código
newman run petshop-api-collection.json -e petshop-api-environment.json

**Contributing**

Contributions are welcome. If you find bugs or have suggestions for improving the collection, please open an issue or submit a pull request.

**License**

The code in this repository is licensed under the Apache License 2.0. See the LICENSE file for details.
For more information about the Petshop API, please refer to the Swagger Documentation.
