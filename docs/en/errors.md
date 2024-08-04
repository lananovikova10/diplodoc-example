# Common Errors

- NetworkException: Indicates network connectivity issues.
- TimeoutException: Indicates that the request timed out.
- ServerException: Indicates an error response from the server.

## Handling Errors
Use try-catch blocks to handle exceptions effectively:

```kotlin
import kotlinx.coroutines.flow.catch

fun main() = runBlocking {
    val client = HttpClient()
    client.get("https://api.example.com/data")
        .catch { e -> println("Error: ${e.message}") }
        .collect { response -> println(response) }
}

```
