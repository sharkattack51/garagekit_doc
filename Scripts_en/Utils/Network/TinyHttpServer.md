# TinyHttpServer

Run a simple web server inside Unity.

```csharp
namespace GarageKit
public class TinyHttpServer : MonoBehaviour
```

#### Inheritance

`TinyHttpServer` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/tinyhttpserver_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|listenOnStart|bool|Start server with Start()|
|port|int|Port number|

#### Methods

Response callback
```csharp
public HttpResponce OnHttpRequest
```

Start web server
```csharp
public void StartServer()
```

Stop web server
```csharp
public void StopServer()
```
