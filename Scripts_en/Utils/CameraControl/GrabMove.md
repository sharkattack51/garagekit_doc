# GrabMove

Move objects using multitouch grab operations. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
public class GrabMove
```

#### Inheritance

`GrabMove` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/grabmove_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|renderCamera|Camera|Camera for hit detection|
|grabTouchNum|int|Number of touches for judgment during multitouch operation|
|moveBias|float|Movement amount|
|smoothTime|float|Movement smooth amount|
|disableComponents|MonoBehaviour[]|Components to be turned off by combination operations|

#### Methods

Check input lock
```csharp
public bool IsInputLock { get; }
```

Lock input
```csharp
public void LockInput(object sender)
```

Unlock input
```csharp
public void UnlockInput(object sender)
```

Reset to initial position
```csharp
public void ResetGrabMove()
```
