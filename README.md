We have a simple Bitcoin exchange API https://blockchain.info/api/exchange_rates_api there are two endpoints that we would like you to use to complete tasks 1 & 2. N.B. You have 1 hour to complete as much of this exercise as possible, don’t worry if you don’t complete it!!.  Please use whichever libraries/frameworks and online resources you deem appropriate to complete this exercise.

Task 1
------
 
*  Using Java, build a Web Application that GETs the ticker information back from the endpoint ( https://blockchain.info/ticker ) and sorts the response by 15m in ascending order  and in an organised way present this information back in browser using Semantic HTML. It is expected that you will also style your markup, the look and feel is left for you, although basic responsiveness is expected.  For the purpose of this exercise the should work in the latest copy of Chrome.


*  This information changes every few seconds, please build in an Ajax mechanism for updating and displaying the latest available information on a 3 second recurring basis. 

Do not worry about JS build tooling for this exercise.

 
Task 2 - ( stretch goal )
------
 
Include a basic form to allow a user to perform a currency conversion from one of the currencies returned from step 1 only and then display the resulting value.  N.B. it is not expected that you calculate this client-side, instead please add an endpoint in your Java app that proxies through to https://blockchain.info/tobtc?currency=CUR&value=20

* I Should not be able to request a currency that does not feature in the response from Task 1
* The amount should be numeric only
* The amount that I wish to convert should be greater than 0 and less than 1,000,000 in the selected currency

If I supply an invalid set of request values then I should be notified and the API request should not happen.
