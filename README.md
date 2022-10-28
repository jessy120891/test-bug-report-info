# Bugs_Reports   

## API_2

### ID 
001
### Status:
New

### Title:
It does not return the correct code_tate when executing a POST method

### Summary: 
Executing a POST method on this URL is expected to return a 500 error code.The POST method is not allowed because it is a URL that only supports the GET method. This returns a Recaptcha link.

### Data:
URL: https://www.google.com/recaptcha/api2/webworker.js?hl=en&v=ovmhLiigaw4D9ujHYlHcKKhP

### Reproduction Steps:
1. Start the client to run API tests (Postman/PythonScripts).
2. Invoke the REST API call using the POST method.
3. Examine the status_code returned by the Rest API

### Expected Result:
      Status Code = 500 Internal Server Error
      
### Actual Result:
       Status Code = 405 Method Not Allowed
       
### Defect Environment:
Production environment API version: 
* Postman version v10
* Consult REDME.md file for configuration and versions of Python scripts

### Priority:
Blocker

### Attachments:

![Postman_Capture_001](https://user-images.githubusercontent.com/88491723/198715447-711bd8d6-31cd-4bd5-8d2a-f006d89554d0.JPG)
![Python_Capture_001](https://user-images.githubusercontent.com/88491723/198715478-f68ee16d-e5b8-43a7-989d-08a9a1d35eae.JPG)




### ID 
002
### Status:
New

### Title:
Within the API response it does not return "SQL error"

### Summary: 
When executing the post method for the provided API, the message indicated in the requirements is not returned within the response elements.

### Data:
URL: https://www.google.com/recaptcha/api2/webworker.js?hl=en&v=ovmhLiigaw4D9ujHYlHcKKhP

### Reproduction Steps:
1. Start the client to run API tests (Postman/PythonScripts).
2. Invoke the REST API call using the POST method.
3. Check within the elements that it returns if the message "SQL error" appears

### Expected Result:
      Find in the elements that are returned in the response the message "SQL error"
      
### Actual Result:
       Does NOT return the expected message in any of the elements
       
### Defect Environment:
Production environment API version:
API version: 
* Postman version v10
* Consult REDME.md file for configuration and versions of Python scripts

### Priority:
Major

### Attachments:
![Postman_Capture_001](https://user-images.githubusercontent.com/88491723/198716933-2a43891d-1da8-441c-b9d8-8503d66e7216.JPG)
![Python_Capture_001](https://user-images.githubusercontent.com/88491723/198717009-ec21fc18-2481-42ce-9e87-a27e4afdb9a6.JPG)


## API_1

### ID 
003
### Status:
New

### Title:
"isUtilizingAdvertiser1pEnabled" key is not returning the expected value

### Summary: 
When executing a GET method to obtain a specific value for the key "isUtilizingAdvertiser1pEnabled" within the JSON, it returns an unexpected value

### Data:
URL: https://ct.pinterest.com/user/?event=search&ed=%7B%22np%22%3A%22gtm%22%7D&tid={today_date.timestamp()}&cb={next_date.timestamp()

### Reproduction Steps:
1. Start the client to run API tests (Postman/PythonScripts).
2. Invoke the REST API call using the GET method
3. Verify in the JSON that the API responds the value to the key "isUtilizingAdvertiser1pEnabled"

### Expected Result:
      The expected value for the key "isUtilizingAdvertiser1pEnabled" is FALSE
      
### Actual Result:
       The value returned by the key "isUtilizingAdvertiser1pEnabled" is TRUE
       
### Defect Environment:
Production environment API version:
* Postman version v10
* Consult REDME.md file for configuration and versions of Python scripts

### Priority:
Major

### Attachments:
![Postman_Capture_003](https://user-images.githubusercontent.com/88491723/198718857-37b9c1a7-b137-48a7-ab33-9a662b59beec.JPG)
![Python_Capture_003](https://user-images.githubusercontent.com/88491723/198718886-aecd85ee-5343-496f-9808-6f53663021ba.JPG)




