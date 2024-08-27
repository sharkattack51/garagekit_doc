# FlyThroughCamera

Perform flythrough operation of the camera by dragging. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class FlyThroughCamera
```

#### Inheritance

`FlyThroughCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/flythroughcamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|groundCollider|Collider|Collider for ground determination|
|limitAreaCollider|Collider|Collider for movement restriction|
|useLimitArea|bool|Movement restriction settings|
|moveBias|float|Movement amount|
|moveSmoothTime|float|Movement smooth amount|
|dragInvertX|bool|Horizontal drag direction reversal setting|
|dragInvertY|bool|Vertical drag direction reversal setting|
|rotateBias|float|Directional rotation amount|
|rotateSmoothTime|float|Directional rotation smooth amount|
|rotateInvert|bool|Direction rotation reversal setting|
|combinationOrbitCamera|[OrbitCamera](~/Scripts_en/Utils/CameraControl/OrbitCamera.md)|Target component for combination operation|

#### Enums

##### __FLYTHROUGH_CONTROLL_TYPE__

|enums|description|
|:--|:--|
|DRAG|Move by dragging|
|DRAG_HOLD|Move by holding after dragging|

##### __FLYTHROUGH_MOVE_TYPE__

|enums|description|
|:--|:--|
|XZ|XZ plane operation|
|XY|XY plane operation|

#### Methods

Get hierarchy root
```csharp
public GameObject FlyThroughRoot { get; }
```

Get root for position shift
```csharp
public Transform ShiftTransform { get; }
```

Get current position
```csharp
public Vector3 currentPos { get; }
```

Get current rotation
```csharp
public Quaternion currentRot { get; }
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

Move camera flythrough to the target position
```csharp
public void MoveToFlyThrough(Vector3 targetPosition, float time = 1.0f)
```

Instantly move camera by a specified amount
```csharp
public void TranslateToFlyThrough(Vector3 move)
```

Rotate camera flythrough towards the target
```csharp
public void RotateToFlyThrough(float targetAngle, float time = 1.0f)
```

Move camera flythrough by specified amount
```csharp
public void PushMove(Vector3 move)
```

Rotate camera flythrough by a specified amount
```csharp
public void PushRotate(float rotate)
```

Reset camera position and rotation
```csharp
public void ResetFlyThrough()
```

#### Example

- /Scenes/Examples/CameraControllExample.unity
