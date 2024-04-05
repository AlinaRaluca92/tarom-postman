# API Testing Project for Tarom-postman

 The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

##### Application under test: Tarom

##### Tools used: Postman, Newman

##### Collection link: (https://github.com/AlinaRaluca92/tarom-postman/blob/main/Tarom.postman_collection.json)

#### Get Flight Details

##### HTTP method for request: GET

##### Request description: 
This request is used to retrieve details about a specific flight, including destination, departure time, arrival time, available seat count, etc. The API documentation specifies that this request should include the flight_number parameter in the URL to specify the desired flight.

##### Test types / techniques used:  
Integration Testing: To ensure that the request works correctly within the application context.
Expected Testing: Verifying that all returned flight details match the expected values from the database.
Performance Testing: Measuring the server response time to evaluate the request's performance.
##### Response status code: 200 OK

Below you can find a picture of the API request from Postman:


