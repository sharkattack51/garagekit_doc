# ObjectOrbit

Orbit rotates the object around the target by dragging. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
public class ObjectOrbit
```

#### Inheritance

`ObjectOrbit` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/objectorbit_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|sensitivity|float|Operation sensitivity|
|speed|float|Rotation speed|
|smoothTime|float|Rotation smooth amount|
|clampRotationX|bool|X rotation limit|
|clampRotationX_Min|float|X rotation limit min|
|clampRotationX_Max|float|X rotation limit max|
|invertDragX|bool|Horizontal drag direction reversal setting|
|invertDragY|bool|Vertical drag direction reversal setting|

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

Reset orbit rotation
```csharp
public void ResetOrbit()
```