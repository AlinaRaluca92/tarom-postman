# API Testing Project for Tarom-postman

 The scope of this project is to use all API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

##### Application under test: Tarom

##### Tools used: Postman, Newman

##### Collection [link](https://github.com/AlinaRaluca92/tarom-postman/blob/main/Tarom.postman_collection.json)

# Tests performed

#### 1.Get Flight Details

##### HTTP method for request: GET

##### Request description: 
This request is used to retrieve details about a specific flight, including destination, departure time, arrival time, available seat count, etc. The API documentation specifies that this request should include the flight_number parameter in the URL to specify the desired flight.

##### Test types / techniques used:  
Integration Testing: To ensure that the request works correctly within the application context.
Expected Testing: Verifying that all returned flight details match the expected values from the database.
Performance Testing: Measuring the server response time to evaluate the request's performance.
##### Response status code: 200 OK

Below you can find a picture of the API request from Postman:

![Api request](https://github.com/AlinaRaluca92/tarom-postman/blob/main/Request%20from%20Postman.JPG)


##### JavaScript Tests:


![JavaScipt Tests](https://github.com/AlinaRaluca92/tarom-postman/blob/main/Java%20script%20test.JPG)

####  2. Get Airport Details

##### HTTP method for request: GET

#####  Request description: 
This request is used to retrieve details about a specific airport, such as its name, location, code, and facilities. According to the API documentation, this request requires the airport_code parameter to be included in the URL to specify the desired airport.

#####  Test types / techniques used:

Integration Testing: Ensuring that the request functions correctly within the application environment.

Expected Testing: Verifying that all returned airport details align with the expected values stored in the database.

Performance Testing: Measuring the server's response time to evaluate the request's performance.

#####  Response status code: 200 OK

Below you can find a picture of the API request from Postman:

![](https://github.com/AlinaRaluca92/tarom-postman/blob/main/Request%20from%20Postman.JPG)

![](https://github.com/AlinaRaluca92/tarom-postman/blob/main/test%20results.JPG)

####  3. Check Flight Delay

#####  HTTP method for request: GET

##### Request description: 
This request is used to check if a specific flight is delayed. It takes the flight_number as a parameter to identify the flight for which delay information is requested.

##### Test types / techniques used:

Functional Testing: Verifying that the delay information returned is accurate and reflects the current status of the flight.

Boundary Testing: Testing the request with various flight numbers, including valid and invalid ones, to ensure the system handles them appropriately.

Error Handling Testing: Verifying that the system returns meaningful error messages for invalid inputs or when the requested flight information is not available.

#####  Response status code: 200 ok 


Below you can find a picture of the API request from Postman:


![](https://github.com/AlinaRaluca92/tarom-postman/blob/main/RP.JPG)

# Execution report for the created API collection

#####  Below you can find the execution report that was generated through the Postman collection runner.   

![](https://github.com/AlinaRaluca92/tarom-postman/blob/main/execution%20report.JPG)

# Defects found

Defects that can be encountered in Postman while testing the Tarom application's API may vary based on the specific endpoints being tested and the complexity of the application. Here are some common types of defects that could be encountered:

Incorrect Data: The API may return incorrect data for certain requests. This could include incorrect flight details, airport information, or delay status.

Server Errors: The API might encounter server errors (5xx status codes) due to issues on the server-side, such as database connection problems or internal server failures.

Missing Data: Some requests may return incomplete data or omit certain expected fields. This could result in missing information in the API response.

# Conclusions

In conclusion, while the Tarom application's API in Postman demonstrates adequate functionality and usability, there are areas for improvement to enhance reliability, performance, and user experience. By addressing these areas and diligently addressing identified defects, the Tarom application can better meet the needs of its users and provide a more seamless experience for accessing flight information.


