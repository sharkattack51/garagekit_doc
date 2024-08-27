# ExternalProcess

Start an external process.

```csharp
namespace GarageKit
public class ExternalProcess : MonoBehaviour
```

#### Inheritance

`ExternalProcess` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/externalprocess_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|exePath|string|Executable file path|
|pathFromStreamingAssets|bool|Load flag from StreamingAssets|
|arguments|string|Execute parameter arguments|
|startupOnStart|bool|Autorun flag on `Start()`|
|showWindow|bool|Window display when running a process|

#### Methods

Get internal process ID
```csharp
public int ProcId { get; }
```

Process execution state
```csharp
public bool IsRunning { get; }
```

Start the process
```csharp
public void StartProcess()
```
