# ObjectOrbit2

Orbit rotates the object around the target by dragging. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
public class ObjectOrbit2
```

#### Inheritance

`ObjectOrbit2` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/objectorbit2_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|renderCam|Camera|Hit judgment camera|
|sensitivity|float|Operation sensitivity|
|smoothTime|float|Rotation smooth amount|
|invertRot|bool|Rotation direction reversal setting|
|collidRadiusFromBounds|bool|Automatically set the judgment collider size from the bounding|
|collidRadius|float|Collider radius for judgment|

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
