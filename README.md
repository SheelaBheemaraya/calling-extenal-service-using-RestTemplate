# calling-extenal-service-using-RestTemplate
#Invoking currency-exchange-service from currency-conversion-service

# Invoking currency-exchange-service from currency-conversion-service


A RestTemplate instance is thread-safe and can be used to access any number of services in different parts of your application.


Note:run both the application independently

 -->for h2 console : http://localhost:8000/h2-console
-->Get Request: http: //localhost:8000/currency-exchange/from/USD/to/INR. 
 response:
{  
id: 101,  
from: "USD",  
to: "INR",  
conversionMultiple: 72,  
port: 8000  
}  
------------------------------------------------------------------------------------------------------------------------------------------------------>---
-->Get request:http://localhost:8100/currency-converter/from/USD/to/INR/quantity/100

{  
Id: 101,  
from: "USD",  
to: "INR",  
conversionMultiple: 72,  
quantity: 100  
totalCalculatedAmount: 7200,  
port: 8000  
}  
