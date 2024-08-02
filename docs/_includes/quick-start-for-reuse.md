## Quick Start

use the any http method suspend function:

```
runBlocking {
    val string: String = Fuel.get("https://publicobject.com/helloworld.txt").body.string()
    println(string)
}

runBlocking {
    val string: String = "https://publicobject.com/helloworld.txt".httpGet().body.string()
    println(string)
}

runBlocking {
    val fuel = FuelBuilder().build()
    val string: String = fuel.get(request = { url = "https://publicobject.com/helloworld.txt" }).body.string()
    println(string)
}
```