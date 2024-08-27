# UDPReceiver

UDP 通信の受信をします。

```csharp
namespace GarageKit
public class UDPReceiver : MonoBehaviour
```

#### Inheritance

`UDPReceiver` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/udpreceiver_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|port|int|受信ポート番号|
|autoStart|bool|自動で受信開始|

#### Methods

最新の受信文字列
```csharp
public string LatestReceivedDataStr { get; }
```

最新の受信バイトデータ
```csharp
public byte[] LatestReceivedDataBytes { get; }
```

文字列での受信コールバック
```csharp
public Action<string> OnReceived
```

バイトデータでの受信コールバック
```csharp
public Action<byte[]> OnReceivedBytes
```

ポートを開く
```csharp
public void Open()
```

ポートを閉じる
```csharp
public void Close()
```
