# API reference

`HttpClient`

#|
|| **Request type** | **Definition** ||
|| get(url: String): `Flow<String>` | Performs a GET request and returns the response as a `Flow<String>`. ||
|| post(url: String, body: Any): `Flow<String>` | Performs a POST request with the provided body and returns the response as a `Flow<String>`. ||
|| put(url: String, body: Any): `Flow<String>` | Performs a PUT request with the provided body and returns the response as a `Flow<String>`. ||
|| delete(url: String): `Flow<String>` | Performs a DELETE request and returns the response as a `Flow<String>`. ||
|#

## Response Handling

- `HttpResponse`
Contains properties such as statusCode, headers, and body.


