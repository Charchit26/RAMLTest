# RAMLTest

This is a demo RAML of an API to satisfy the following conditions:
List customers
Create a new customer
Update a customer
Deletes a customerD

The RAML pack was designed using "Desing Center" provided by Mulesoft Anypoint platform.
It has 4 basic CRUD operation capability - GET, POST, PUT and DELETE.

I have tried to use many different RAML features like traits, securitySchemes and includes.

Pagination has also been added to the GET request which adds offset, limit or page in the query parameters to be able to fetch and display only a finite amount of records at one go. This feature is very useful in mobile app development since client does not need to wait too long for large amount of data and requires less bandwidth too.

Caching has been enabled for the GET request too using ETags, which enables the browsers to use the old resource if there was no change made to it by the server, which is evident by the presence of same ETags.

This RAML is extensible to allow additions of more resources like orders, products etc by re-using methods in traits and inheriting from customer's URI parameter "ID".
