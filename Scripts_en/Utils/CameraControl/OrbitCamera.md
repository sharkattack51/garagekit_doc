# OrbitCamera

Rotate the camera around the target by dragging. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class OrbitCamera
```

#### Inheritance

`OrbitCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/orbitcamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|orbitInputType|[ORBIT_INPUT_TYPE](#orbit_input_type)|Operation input type|
|target|GameObject|Rotation center target|
|sensitivity|float|Operation sensitivity|
|smoothTime|float|Rotation smooth amount|
|clampRotationX_Min|float|X rotation limit min|
|clampRotationX_Max|float|X rotation limit max|
|invertDragX|bool|Horizontal drag direction reversal setting|
|invertDragY|bool|Vertical drag direction reversal setting|
|ratioForMouse|float|Rotation amount when operating the mouse|
|combinationFlyThroughCamera|[FlyThroughCamera](~/Scripts_en/Utils/CameraControl/FlyThroughCamera.md)|Target component for combination operation|

#### Enums

##### __ORBIT_INPUT_TYPE__

|enums|description|
|:--|:--|
|PRIMARY|Primary input|
|SECONDARY|Secondary input|

#### Methods

Get hierarchy root
```csharp
public GameObject OrbitRoot { get; }
```

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

#### Example

- /Scenes/Examples/CameraControllExample.unity
