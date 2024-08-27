# TinyHttpServer

Unity 内に簡易 Web サーバーを実行します。

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
|listenOnStart|bool|Start() で開始|
|port|int|ポート番号|

#### Methods

レスポンスコールバック
```csharp
public HttpResponce OnHttpRequest
```

Web サーバーを開始
```csharp
public void StartServer()
```

Web サーバーを停止
```csharp
public void StopServer()
```
