# Week-14-Homework---Web-Development

Ambar Vargas
Cybersecurity Bootcamp
Week 14 Homework:
Web DevelopmentQuestions

HTTP Requests and Responses

1. What type of architecture does the HTTP request and response process occur in?

      Client-Server Architecture, which takes part in OSI layer 7 (the application layer). 



2. What are the different parts of an HTTP request?
  
      The request line, the header, and the whitespace are the different parts of an HTTP request. The request line contains the request method, the name of the requested resource and the version of HTTP in use as well as query parameters. The Headers contain additional information about the requested resource and are used to implement various security measures like authentication. Finally, whitespace indicates the end of the request.



3. Which part of an HTTP request is optional?
  
      The request body, which may contain information such as login credentials used for authentication.


4. What are the three parts of an HTTP response?
  
      The status line, the response header, and the response body.


5. Which number class of status codes represents errors?
  
      The 400’s represent client errors, and the 500’s indicate server errors.


6. What are the two most common request methods that a security professional will encounter?
  
      GET and POST. GET requests ask for data from a server to retrieve data. POST requests send data to a specified resource.


7. Which type of HTTP request method is used for sending data?
  
      The POST method.


8. Which part of an HTTP request contains the data being sent to the server?
  
      The request body. It can contain data ranging from login credentials or files that need to be uploaded.


9. In which part of an HTTP response does the browser receive the web code to generate and style a web page?
  
      The response body. 



Using curl


10. What are the advantages of using curl over the browser?
  
      Using curl is a way to quickly test HTTP requests in a way that can be automated and to make changes simultaneously. This includes testing web security  configurations, testing how secure the servers are (so as not to leak important data), verifying that the servers only reply to specific requests, and checking for/mitigating vulnerabilities.


11. Which curl option is used to change the request method?
  
      curl -X


12. Which curl option is used to set request headers?
  
      curl -H


13. Which curl option is used to view the response header?
  
      curl -i


14. Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?
  
      curl -v



Sessions and Cookies


15. Which response header sends a cookie to the client?
  
      <HTTP?1/1 200 OK>


16. Which request header will continue the client's session?
 
     <GET /cart HTTP/1.1>
  
     <Host: www.example.org>
  
     <Cookie: cart=Bob>
  
    (this get request header includes the site cookie which allows faster and continued access to the server since the user’s data is saved in the cookie). 


Example HTTP Requests and Responses



17. What is the request method?
  
      POST


18. Which header expresses the client's preference for an encrypted response?
 
      <Accept-Encoding: gzip, deflate, br> 


19. Does the request have a user session associated with it?
 
      No, there is no session ID or cookie listed.
  

20. What kind of data is being sent from this request body?
  
      Login credentials for Barbara (They’re coming for you Barbara). 



HTTP Response


21. What is the response status code?
  
      200


22. What web server is handling this HTTP response?
  
      Apache


23. Does this response have a user session associated to it?
  
      Yes, <SessionID=5>


24. What kind of content is likely to be in the [page content] response body?
 
      Some sort of text.


25. If your class covered security headers, what security request headers have been included?
 
      Strict-Transport-Security



Monoliths and Microservices


26. What are the individual components of microservices called?
  
      Front-end server, back-end server, and database are the basic components of a typical web app. Microservices sperate those application components into their own machines, such as a jump-box or DVWA server we used in our project. 


27. What is a service that writes to a database and communicates to other services?
  
      The back-end server, specifically an Application Programming Interface(API), will write and read corresponding data to and from a databases, and communicate to the other services within a network/web application.


28. What type of underlying technology allows for microservices to become scalable and have redundancy?
  
      Application programing interfaces (APIs)



Deploying and Testing a Container Set


29. What tool can be used to deploy multiple containers at once?
 
      Docker


30. What kind of file format is required for us to deploy a container set?
 
      YAML file



Databases


31. Which type of SQL query would we use to see all of the information within a table called customers?
   
    select


32. Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)
  
    Insert into


33. Why would we never run DELETE FROM <table-name>; by itself?
  
    It would delete more than the intended data, which would be disastrous. 
