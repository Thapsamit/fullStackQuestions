# fullStackQuestions

## What is an API?
- API is Application Programming interface that is software intermediary between two applications that allows two application to talk to each other.
- **Types?**
  - SOAP (SIMPLE OBJECT ACCESS PROTOCOL): It defines messages in XML format used by web applications to communicate with each other.
  - REST (Representational State Transfer): It makes use of HTTP to GET, POST, PUT, or DELETE data. It is basically used to take advantage of the existing data.
  
  
## What is RESTAPI?
- Representational State Transfer (REST) is an architectural style that defines a set of constraints to be used for creating web services. 
- REST API is a way of accessing web services in a simple and flexible way without having any processing.
- REST uses less bandwidth, simple and flexible making it more suitable for internet usage. 
- Web services which follow the REST architectural style are known as RESTful web services. 
- Interaction in REST based systems happen through Internet’s Hypertext Transfer Protocol (HTTP). 
- It allows requesting systems to access and manipulate web resources by using a uniform and predefined set of rules.
- Architectural designs:-
  - **uniform interface:-**
    - It suggests that there should be an uniform way of interacting with a given server irrespective of device or type of application.
    - Individual resources are identified in requests. For example: API/users.
    - Client has representation of resource and it contains enough information to modify or delete the resource on the server,
    - Each message includes enough information to describe how to process the message so that server can easily analyses the request.
    - Hypermedia as the Engine of Application State (HATEOAS): It need to include links for each response so that client can discover other resources easily.
  - **Stateless:-** 
    - It means that the necessary state to handle the request is contained within the request itself and server would not store anything related to the session.

  - **Cacheable:-**
    - Every response should include whether the response is cacheable or not and for how much duration responses can be cached at the client side.
  - **Client-Server:** REST application should have a client-server architecture. A Client is someone who is requesting resources and are not concerned with data storage, which remains internal to each server, and server is someone who holds the resources and are not concerned with the user interface or user state.
  - **Layered system:** An application architecture needs to be composed of multiple layers. Each layer doesn’t know any thing about any layer other than that of immediate layer and there can be lot of intermediate servers between client and the end server.



## What is The difference between GraphQL vs RestAPI?
- GraphQL is an alternative to REST for developing APIs, not a replacement.
- The biggest difference between GraphQL and REST is the manner in which data is sent to the client.

| GraphQL | RESTApi |
| ------- | ------- |
| while in GraphQL, the client requests data with queries. |  In a REST architecture, the client makes an HTTP request and data is sent as an HTTP response, |
| In GraphL, you define the object on the client. | the structure of the request object is defined on the server. |
| GraphQL was designed to allow the client to ask for only the data it needs. While the server might be able to deliver more data to the client for a single request, it would only send the data requested by the client. | It uses multiple requests to get different dta |
| GraphQL simplifies the task of aggregating data from multiple sources or APIs and then resolving the data to the client in a single API call.  | On the other hand, API technologies like REST would require multiple HTTP calls to access data from multiple sources. |
| GraphQL exposes a single endpoint that allows you to access multiple resources. | It exposes multiple endpoints to access multiple resources |
| No under or uver fetching of data | May under or over fetch the data |

## When should you use a REST API?
- GraphQL gives clients the power to execute queries to get exactly what they need. But, what if a client sends a query asking for many fields and resources,  therefore areise performance issues.
- For complex queries, a REST API might be easier to design because you can establish multiple endpoints for specific needs,
- The main benefit of using GraphQL is the ability to send a query that specifies only the information you need and receiving exactly that. However, you can achieve this same effect using REST, by passing the name of the fields you want to use in the URL,
- In REST, checking the response status is the only way to know whether the request was executed successfully, if there was a server error, or if the resource was not found. But, when an error occurs in GraphQL, you get something similar to the following:
- You’ll have to parse this message to know if there’s an error, and different errors will probably have slightly different formats or some custom fields.





