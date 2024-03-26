App connects to NBP Web API:http://api.nbp.pl/en.html
This API requests from NBP exchange rates of multiple currencies or single currency
In order to use this API you have to make GET HTTP request with query parameter called currency.
Query parameter currency is currency code in standard ISO 4217

App has three endpoints: 
/rates - returns information on desired currency
/tables - returns table with exchange rates 
/top3 - returns EUR, GBP, USD exchange rates

Example request for rates:
curl --location 'localhost:8081/rates?currency=AUD'

Example request for tables: 
curl --location 'localhost:8081/tables'

Example request for top3: 
curl --location 'localhost:8081/top3'
