## Summary


Learnt about what HTTP is and about how it uses PATHs and METHODs;

HTTP Flow (when the client wants to communicate with a server) (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview#http_flow))

1) TCP connection; this is used to send a request / to receive an answer
2) Send a HTTP message (Example; GET google.ca/cats)

The HTTP methods are;

* GET: used to get some data from the server
* POST: used to create new data
* PUT: used for editing data on the server
* DELETE: used to delete some existing data

Learnt more about the structured of URLs (_Uniform Resource Locator_) (Source: [MDN](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_URL))

Learnt about HTTP responses - ie status codes (HTTP error codes that are returned when a response is given to a request) and the body (data stored in the body of the HTTP response that can be either HTML or JSON). Examples of some common error codes are 404: “Resource was not found”, 500: “The server had an error”, and 451: “Resource unavailable for legal reasons” (Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/451))