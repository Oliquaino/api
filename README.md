# Edelyn's API
This Edelyn's API provides endpoints to manage a simple database of names. It supports operations to create, read, update, and delete records. The API utilizes the Slim framework for routing and PDO (PHP Data Objects) for database interactions.


# API Description
An API, or Application Programming Interface, is a set of rules and protocols that allow different software applications to communicate with each other. It defines the methods and data formats that applications can use to request and exchange information, enabling seamless integration and interaction between various systems.

It offers fundamental functions for adding, retrieving, updating, and deleting name records. Whether you want to insert a new name, find specific names, modify existing ones, or remove entries, this API simplifies the process. It operates on the Slim framework, ensuring smooth and organized navigation, while PDO (PHP Data Objects) provides a secure and reliable way to interact with the database. This combination of technologies not only makes the API robust but also ensures that managing names becomes a seamless task for developers.


## API Endpoints

(POST/postName)
- URL: http://127.0.0.1/api/public/postName
- Purpose: Add a new name to the database.
- HTTP Method: POST
- Necessary Parameters:
  - 'fname' (string): First name.
  - 'lname' (string): Last name.

(GET/getName)
- URL: http://127.0.0.1/api/public/printName
- Purpose: Fetch a list of names from the database.
- HTTP Method: GET

(POST/updateName)
- URL: http://127.0.0.1/api/public/updateName
- Purpose: Modify an existing name entry in the database.
- HTTP Method: POST
- Required Parameters:
  - 'id' (int): The unique identifier of the name.
  - 'fname' (string): New first name.
  - 'lname' (string): New last name.

(POST/deleteName)
- URL: http://127.0.0.1/api/public/deleteName
- Purpose: Remove a name record from the database.
- HTTP Method: POST
- Required Parameters:
  - 'id' (int): The unique identifier of the name to be deleted.


## Request Payload

JSON Payload Name:

JSON Payload postName: Request payload: { "lname":"hortizuela", "fname":"manny" } JSON Payload printName:

Request payload:

JSON Payload updateName:

Request payload: { "id":1, "lname":"wick", "fname":"john" } JSON Payload deleteName:

Request payload: { "id":1 }

 


## Response Payload

JSON Payload Name:

Response payload: { "status":"success","data":null } JSON Payload printName:

Response payload: { "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"] } JSON Payload updateName:

Response payload: { "status":"success","data":null } JSON Payload deleteName:

Response payload: { "status":"success","data":null }




## Usage


To Insert Data into the Database:
1. Open Postman.
2. Choose the HTTP method as "POST."
3. Set the URL to http://127.0.0.1/api/public/postName.
4. In the request body, provide the "fname" and "lname" parameters with the desired values.
5. Click the "Send" button to execute the request.

To Update Existing Data:
1. Launch Postman.
2. Select the HTTP method as "POST."
3. Input the URL as http://127.0.0.1/api/public/updateName.
4. Include the "id," "fname," and "lname" parameters in the request body with the updated values.
5. Click "Send" to submit the request.

To Retrieve Data from the Database:
1. Open Postman.
2. Choose the HTTP method as "GET."
3. Specify the URL as http://127.0.0.1/api/public/printName.
4. Keep the request body empty, as no additional parameters are required.
5. Click "Send" to retrieve the data.

To Delete Data from the Database:
1. Launch Postman.
2. Set the HTTP method to "POST."
3. Enter the URL as http://127.0.0.1/api/public/deleteName.
4. In the request body, include the "id" parameter with the ID of the data you want to delete.
5. Click "Send" to initiate the deletion request.

 


## License

No License.

 


## Contributors


Dr. Manny Hortizuela:
    some codes
    structure of the database
    payloads
    others

 Recelle Ann Orillada
    Collaborator

## Contact Information

Name: Edelyn B. Oliquiano
Email: edelyn.oliquiano@dmmmsu.edu.ph
Contact Number: 09267290837

