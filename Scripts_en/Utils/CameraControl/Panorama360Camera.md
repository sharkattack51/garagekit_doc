# Panorama360Camera

Panoramic 360° camera operation.

```csharp
namespace GarageKit
public class Panorama360Camera
```

#### Inheritance

`Panorama360Camera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/panorama360camera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|mode|[OPERATION_MODE](#operation_mode)|Operation mode|
|rotationSpeed|float|Rotation speed|
|useLimit|bool|Rotation limit setting|
|limitRotL|float|Limit angle for left rotation direction|
|limitRotR|float|Limit angle for right rotation direction|
|invertRotH|bool|Horizontal rotation direction reversal setting|
|invertRotV|bool|Vertical rotation direction reversal setting|
|useSmooth|bool|Rotation smooth setting|
|smoothTime|float|Rotation smooth amount|

#### Enums

##### __OPERATION_MODE__

|enums|description|
|:--|:--|
|GYRO|Gyro operation|
|DRAG_MOUSE|Mouse operation|
|DRAG_TOUCH|Touch operation|
|GAME_PAD|Gamepad operation|

#### Methods

Reset gyro
```csharp
public void ResetGyro()
```

Reset camera rotation
```csharp
public void ResetRotation(bool force = false)
```

Set camera rotation value
```csharp
public void SetRotate(float h, float v, float speed)
```

#### Example

- /Scenes/Examples/CameraControllExample.unity
