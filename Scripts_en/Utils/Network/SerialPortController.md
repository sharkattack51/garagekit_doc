# SerialPortController

Sends and receives serial communications.

> [!IMPORTANT]
> If you want to use it, change ApiCompatibilityLevel in PlayerSettings to `.NET Framework`.

```csharp
namespace GarageKit
public class SerialPortController : MonoBehaviour
```

#### Inheritance

`SerialPortController` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/serialportcontroller_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|autoOpen|bool|Open port automatically|
|autoSearchPort|bool|Automatic search for available port|
|autoSearchInReverse|bool|Automatic backward search for available port|
|portName|List<string>|Port name|

Serial connection parameters

|member|type|description|
|:--|:--|:--|
|baudRate|int|BaudRate|
|parity|Parity|Parity|
|dataBits|int|DataBits|
|stopBits|StopBits|StopBits|
|encoding|Encoding|TextEncoding|
|newLineCode|NewLineCode|NewLineCode|
|handShake|Handshake|Handshake|
|dtrEnable|bool|DtrEnable|
|rtsEnable|bool|RtsEnable|
|readTimeout|int|ReadTimeout|
|writeTimeout|int|WriteTimeout|

#### Enums

##### __NewLineCode__

|enums|description|
|:--|:--|
|LF|\n|
|CR|\r|
|CRLF|\r\n|

#### Methods

Data received callback
```csharp
public Action<string> OnReceive
```

Latest received string
```csharp
public string ReceivedDataStr { get; }
```

Check port status
```csharp
public bool IsOpen { get;}
```

Find and open port
```csharp
public bool TryRecursiveOpen()
```

Open port
```csharp
public void Open()
```

Close port
```csharp
public void Close()
```

Send string command
```csharp
public void SendCommand(string str)
```

Send string command asynchronously
```csharp
public async UniTask SendCommandAsync(string str)
```

Convert string command to byte data and send
```csharp
public void SendCommandByte(string str)
```

Convert string command to byte data and send asynchronously
```csharp
public async UniTask SendCommandByteAsync(string str)
```

Convert command array of space separated numbers to hexadecimal and send
```csharp
public void SendCommandArrayHexByte(string str)
```

Convert command array of space separated numbers to hexadecimal and send asynchronously
```csharp
public async UniTask SendCommandArrayHexByteAsync(string str)
```

Send byte data
```csharp
public void SendByte(byte[] strBytes)
```

Send byte data asynchronously
```csharp
public async UniTask SendByteAsync(byte[] strBytes)
```
