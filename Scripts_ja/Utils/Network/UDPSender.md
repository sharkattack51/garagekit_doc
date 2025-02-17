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
public void Send(string dataStr, string address = null, int? port = null, CancellationToken ct = default(CancellationToken))
```

バイトデータの送信
```csharp
public void Send(byte[] data, string address = null, int? port = null, CancellationToken ct = default(CancellationToken))
```

文字列の複数回送信
```csharp
public void TryContinuousSend(string dataStr, int tryCount, float span = 0.1f, string address = null, int? port = null, CancellationToken ct = default(CancellationToken))
```

指定アドレス範囲への文字列の送信
```csharp
public void RangeSend(string dataStr, List<string> addresses, int? port = null, CancellationToken ct = default(CancellationToken))
public void RangeSend(string dataStr, string startAddress, int addressNum, int? port = null, CancellationToken ct = default(CancellationToken))
```

指定アドレス範囲への文字列の複数回送信
```csharp
public void TryContinuousRangeSend(string dataStr, List<string> addresses, int tryCount, float span = 0.1f, int? port = null, CancellationToken ct = default(CancellationToken))
public void TryContinuousRangeSend(string dataStr, string startAddress, int addressNum, int tryCount, float span = 0.1f, int? port = null, CancellationToken ct = default(CancellationToken))
```

文字列のブロードキャスト送信
```csharp
public void Broadcast(string dataStr, int? port = null, CancellationToken ct = default(CancellationToken))
```

バイトデータのブロードキャスト送信
```csharp
public void Broadcast(byte[] data, int? port = null, CancellationToken ct = default(CancellationToken))
```

文字列の複数回ブロードキャスト送信
```csharp
public void TryContinuousBroadcast(string dataStr, int tryCount, float span = 0.1f, int? port = null, CancellationToken ct = default(CancellationToken))
```
