# ARSessionStartHelper

Helper class for the ARSession component. Automatically manages installation confirmation of the AR system on the device and start of an AR session.

> [!IMPORTANT]
> When using it, please enable #define definition in the source code.

```csharp
namespace GarageKit.ARFoundationExtention
[RequireComponent(typeof(ARSession))]
public class ARSessionStartHelper : MonoBehaviour
```

#### Inheritance

`ARSessionStartHelper` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arsessionstarthelper_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|arSession|ARSession|ARSession reference|

#### Methods

AR system initialization fails callback
```csharp
public Action OnFailARSession
```

Callback when requesting installation of AR library (ARCore)
```csharp
public Action OnRequestARLibInstall
```

AR system initialization completion callback
```csharp
public Action OnReadyAR
```
