# kinetik
A lightweight HTTP 2.0 server with an emphasis on speed

## PHASE I
The goal is an HTTP 2.0 static file server.  If `127.0.0.1/readme.text`
is the URL supplied, the HTTP 2.0 static server should:
- return the contents of readme.txt if it is in the document root with HTTP code 200 OK
- return 404 NOT FOUND if it is not in the document root
- return 403 ACCESS DENIED if folder permissions hinder the file from being read  
  
Additionally, kinetik should handle requests and responses signficantly more rapidly than 
Apache and Nginx currently do.  Metrics should be taken to demonstrate this.

## PHASE II
Dynamic web application support (perhaps including a microframework, Chakra integration, 
and an in-memory database?)

## PHASE III
HTTPS support

## RFC
Review this: https://tools.ietf.org/html/draft-ietf-httpbis-http2-04

## Code Style Guidelines
To contribute code, your code must conform to these guidelines:
- namespaces and variables are `lowercased`
- constants are `ALLCAPS`
- classes are `PascalCase`
- functions are `camelCase`
- functions should be less than 70 lines of code
- all `if` statements require brackets
- use properties instead of getters and setters
- use generics instead of type casting

## Pull Requests
Pull requests to fulfill featured items are welcome, but must  
1) be a separate branch from the main one,  
2) conform to the above code style guidelines, and  
3) have unit tests passing at least on Windows
