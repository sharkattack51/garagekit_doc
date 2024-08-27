# UDPSender

Sends UDP communication.

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
|address|string|Destination address|
|port|int|Destination port number|

#### Methods

Send string
```csharp
public void Send(string dataStr, string address = null, int? port = null)
```

Send byte data
```csharp
public void Send(byte[] data, string address = null, int? port = null)
```

Send string multiple times
```csharp
public void TryContinuousSend(string dataStr, int tryCount, float span = 0.1f, string address = null, int? port = null)
```

Broadcast string
```csharp
public void Broadcast(string dataStr, int? port = null)
```

Broadcast byte data
```csharp
public void Broadcast(byte[] data, int? port = null)
```

Broadcast string multiple times
```csharp
public void TryContinuousBroadcast(string dataStr, int tryCount, float span = 0.1f, int? port = null)
```
