# api-testing-with-postman

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: NAVNATH VISHNU CHAVAN

*INTERN ID*: CT08THZ

*DOMAIN*: SOFTWARE TESTING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

## DISCRIPTION OF PROJECT:

Task: To test rest api using postman for functionalalities like authentication and data retrieval.

To perform this actions I have created a collection in which agin I created a get request to try to get data without proper authentication and the result was fail because 
without authentication getting data was not possible so next I re-run the get request with proper authentication and this time result was pass.

For second scenarion I need to create some data so later on I can retrive that data. So for that I performed post reqest and provide some data 
and then by using get requst I retrived the data from api and compleated the tests. And the result was by following:

### **Summary of API Testing Results in Postman**

The Postman test results for the collection **"api-testing-with-postman"** show the execution of three API requests:  

1. **GET Request - Get data with Authentication**  
   - **Endpoint:** `https://api.github.com/user/repos`  
   - **Status:** Passed ✅  
   - **Response Code:** `200 OK`  
   - **Response Time:** `577 ms`  
   - **Response Size:** `3.651 KB`  
   - **Remarks:** The request successfully authenticated and retrieved the list of repositories from GitHub.

2. **POST Request - Post data for data retrieval**  
   - **Endpoint:** `https://rahulshettyacademy.com/Library/Addbook.php`  
   - **Status:** Passed ✅  
   - **Response Code:** `200 OK`  
   - **Response Time:** `195 ms`  
   - **Response Size:** `461 B`  
   - **Remarks:** The request successfully posted the data to the specified endpoint, confirming that the book addition was processed correctly.

3. **GET Request - Data Retrieval**  
   - **Endpoint:** `https://rahulshettyacademy.com/Library/GetBook.php?AuthorName=Navnath Chavan`  
   - **Status:** No tests found  
   - **Response Code:** `200 OK`  
   - **Response Time:** `120 ms`  
   - **Response Size:** `558 B`  
   - **Remarks:** The request was executed successfully, but no validation tests were applied to verify the response.

### **Overall Test Run Statistics**
- **Total Tests Executed:** 2  
- **Passed:** 2  
- **Failed:** 0  
- **Skipped:** 0  
- **Iterations:** 1  
- **Total Duration:** `1.828s`  
- **Average Response Time:** `297 ms`  

### **Key Observations**
1. **Successful Authentication:** The first GET request to GitHub API returned a `200 OK` response, indicating successful authentication and data retrieval.  
2. **Successful Data Posting:** The POST request to the library API successfully added data, suggesting that the API is functioning correctly for data submission.  
3. **No Tests Defined for Data Retrieval:** The last GET request executed correctly, but no assertions or validation checks were present to verify the retrieved data.  

### **Recommendations**
- **Add Test Assertions for Data Retrieval:** Implement response validation to ensure that the retrieved data matches expected values.  
- **Improve Error Handling:** Include tests for scenarios where incorrect or missing data is provided to see how the API responds.  
- **Optimize Response Time:** While response times are within acceptable limits, further optimizations can be explored if needed.  

