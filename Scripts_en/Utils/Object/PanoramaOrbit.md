# PanoramaOrbit

Orbit rotates panoramic objects. If you want to rotate the camera, you can also use [Panorama360Camera](~/Scripts_en/Utils/CameraControl/Panorama360Camera.md).

```csharp
namespace GarageKit
public class PanoramaOrbit : MonoBehaviour, ILocalize
```

#### Inheritance

`PanoramaOrbit` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/panoramaorbit_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|mode|[OPERATION_MODE](#operation_mode)|Operation mode|
|rotationSpeed|float|Rotation speed|
|invertY|bool|Invert Y axis rotation|
|invertX|bool|Invert X axis rotation|

#### Enums

##### __OPERATION_MODE__

|enums|description|
|:--|:--|
|ROTATE_Y|Y axis rotation operation|
|ROTATE_XY|Y and Y axis rotation operation|

#### Methods

Reset rotation
```csharp
public void RotationReset()
```

Set rotate value
```csharp
public void SetRotate(float h, float v, float speed)
```
