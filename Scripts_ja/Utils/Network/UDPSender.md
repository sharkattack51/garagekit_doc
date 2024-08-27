# UDPSender

UDP 通信の送信をします。

```csharp
namespace GarageKit
public class UDPSender : MonoBehaviour
```

#### Inheritance

`UDPSender` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/udpsender_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|address|string|送信先アドレス|
|port|int|送信先ポート番号|

#### Methods

文字列の送信
```csharp
public void Send(string dataStr, string address = null, int? port = null)
```

バイトデータの送信
```csharp
public void Send(byte[] data, string address = null, int? port = null)
```

文字列の複数回送信
```csharp
public void TryContinuousSend(string dataStr, int tryCount, float span = 0.1f, string address = null, int? port = null)
```

文字列のブロードキャスト送信
```csharp
public void Broadcast(string dataStr, int? port = null)
```

バイトデータのブロードキャスト送信
```csharp
public void Broadcast(byte[] data, int? port = null)
```

文字列の複数回ブロードキャスト送信
```csharp
public void TryContinuousBroadcast(string dataStr, int tryCount, float span = 0.1f, int? port = null)
```
