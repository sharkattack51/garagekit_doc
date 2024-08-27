# UDPReceiver

Receives UDP communication.

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
|port|int|Receive port number|
|autoStart|bool|Start receiving automatically|

#### Methods

Latest received string
```csharp
public string LatestReceivedDataStr { get; }
```

Latest received byte data
```csharp
public byte[] LatestReceivedDataBytes { get; }
```

Receive callback in string
```csharp
public Action<string> OnReceived
```

Receive callback with byte data
```csharp
public Action<byte[]> OnReceivedBytes
```

Open port
```csharp
public void Open()
```

Close port
```csharp
public void Close()
```
