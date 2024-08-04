# Configuring Timeouts

Customize connection and read timeouts with `HttpClientConfig`:

```kotlin
import com.example.kotlinstream.HttpClientConfig

val config = HttpClientConfig().apply {
    connectionTimeout = 10000 // 10 seconds
    readTimeout = 10000 // 10 seconds
}

val client = HttpClient(config)
```

