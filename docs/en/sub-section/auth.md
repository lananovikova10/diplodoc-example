# Authentication

For authenticated requests, use the `AuthenticationInterceptor`:

```kotlin
import com.example.kotlinstream.AuthenticationInterceptor

val interceptor = AuthenticationInterceptor("Bearer your-token")

val client = HttpClient().apply {
    addInterceptor(interceptor)
}
```