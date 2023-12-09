# AZ-lac-AsyncDemo
## Azure Logic App Demo of an Asynchronous Request & Response

Logic demo of the Asynchronous pattern HTTP Request and Response Azure Logic App.

Logic app will return an HTTP 202 Accepted with a status URL to poll for run status.

After 5 minute delay the status URL will return 202 OK with a response body.

### Deploy the HTTP Async Demo Logic App 
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fanthonyblake%2FAZ-lac-AsyncDemo%2Fmain%2Ftemplate.json)

### Postman collection to Test

Import the postman collection from **postman/AsyncDemo.postman_collection.json**.

Create 2 Environment Variables in the postman environment.

**async_demo_url** - enter the URL from the HTTP request trigger when the logic app is deployed.
**get_status_url** - will automatically populate with the status URL from the initial logic app 202 response.
