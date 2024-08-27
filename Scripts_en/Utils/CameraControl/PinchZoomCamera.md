# PinchZoomCamera

Camera zoom using multitouch pinch operation. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class PinchZoomCamera
```

#### Inheritance

`PinchZoomCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/pinchzoomcamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|zoomType|[PINCH_ZOOM_TYPE](#pinch_zoom_type)|Zoom processing type|
|zoomBias|float|Zoom amount|
|zoomSmoothTime|float|Zoom smooth amount|
|invertZoom|bool|Zoom direction reversal setting|
|limitMinMaxForRelativePosZ|[LimitValue](#limitvalue)|Relative value limit for Z position|
|limitMinMaxForFOV|[LimitValue](#limitvalue)|FOV value limit|
|limitMinMaxForOrthoSize|[LimitValue](#limitvalue)|Ortho camera size value limit|
|disableComponents|MonoBehaviour[]|Components to be turned off by combination operations|
|zoomToPinchCenterFor2D|bool|Set the center of 2D zoom to the pinch coordinate center|
|ratioForWheel|float|Zoom amount with mouse wheel|

#### Enums

##### __PINCH_ZOOM_TYPE__

|enums|description|
|:--|:--|
|POSITION_Z|Zoom by Z position|
|FOV|Zoom by FOV value|
|ORTHOSIZE|Zoom by ortho camera size|

#### Methods

Current zoom value
```csharp
public float currentZoom { get; }
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

Zoom by specified amount
```csharp
public void PushZoom(float zoomDelta)
```

Zoom to target value
```csharp
public void SetToPinchZoom(float zoom, float time = 1.0f)
```

Reset zoom value
```csharp
public void ResetPinchZoom()
```

#### Example

- /Scenes/Examples/CameraControllExample.unity

---

# LimitValue

Limit value structure

```csharp
namespace GarageKit
[Serializable]
public class LimitValue
```

#### Properties

|member|type|description|
|:--|:--|:--|
|min|float|Min value|
|max|float|Max value|
