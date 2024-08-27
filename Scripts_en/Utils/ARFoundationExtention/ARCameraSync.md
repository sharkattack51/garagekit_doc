# ARCameraSync

Synchronize AR camera objects and parameters.

> [!IMPORTANT]
> When using it, please enable #define definition in the source code.

```csharp
namespace GarageKit.ARFoundationExtention
[RequireComponent(typeof(Camera))]
public class ARCameraSync : MonoBehaviour
```

#### Inheritance

`ARCameraSync` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arcamerasync_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|arCameraManager|ARCameraManager|ARCameraManager reference|
|syncFov|bool|Camera FOV sync settings|
|syncPosition|bool|Camera position sync settings|
|syncRotation|bool|Camera rotation sync settings|
|asLocal|bool|Sync as local coordinate|
