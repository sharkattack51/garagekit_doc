# VRGazeGuideArrow

Controls the display of eye guide arrows in VR.

```csharp
namespace GarageKit
public class VRGazeGuideArrow : MonoBehaviour
```

#### Inheritance

`VRGazeGuideArrow` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/vrgazeguidearrow_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|viewCamera|Camera|HMD camera reference|
|smoothTime|float|Smooth moving amount|
|screenRatio|float|Screen range where guides are enabled|
|arrows|GameObject[]|Arrow object|
|modeGreen|Color32|Green mode color|
|modeRed|Color32|Red mode color|
|useArrow|bool|Arrow display settings|

#### Enums

##### __COLOR_MODE__

|enums|description|
|:--|:--|
|GREEN|Green mode|
|RED|Red mode|

#### Methods

Check if HMD device is in use
```csharp
public bool IsDevicePresent()
```

Change color mode
```csharp
public void ChangeColor(COLOR_MODE mode)
```
