Contains the MicroServer class: is a server implementation that uses the Spark framework to handle HTTP requests and serve responses.
- request validation
- JSON processing
- logging functionalities
- HTTP & HTTPS support

### Workflow Example
1. **Client Request:**
    - Client sends a `POST` request to `/api/config` or `/api/distances` with a JSON body.
2. **Request Handling:**
    - The request information is validated against a schema.
    - JSON is parsed into a specific `Request` object.
    - `buildResponse()` method is called on the `Request` object to prepare the response.
3. **Response Preparation:**
    - Response is turned into JSON then sent to the client.
    - Logging is performed for debugging and monitoring.
4. **Error Handling:**
    - If validation fails a HTTP status code is returned logging the error.