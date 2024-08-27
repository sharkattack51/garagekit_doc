# UrbanViewerLikeCamera

Use the mouse, touch, or game pad to move the camera forward, backward, up, down, left, and right, and to rotate left and right.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
public class UrbanViewerLikeCamera
```

#### Inheritance

`UrbanViewerLikeCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/urbanviewerlikecamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|childCamera|Camera|Child camera in hierarchy to control|
|moveSpeed|float|Movement speed|
|rotateSpeed|float|Rotation speed|
|updateEnable|bool|Update value by Update()|
|primaryDragType|[DragType](#dragtype)|Operation target of primary input (left drag/one finger operation)|
|secondaryDragType|[DragType](#dragtype)|Operation target of secondary input (right drag/two finger operation)|
|tertiaryDragType|[DragType](#dragtype)|Operation target of tertiary input (middle drag/three finger operation)|
|camMoveSpeedForPad|float|Movement speed when using the gamepad|
|camRotSpeedForPad|float|Rotation speed when operating the gamepad|
|invertCamRotXForPad|bool|X rotation direction reversal setting when operating the gamepad|
|invertCamRotYForPad|bool|Y rotation direction reversal setting when operating the gamepad|
|padType|[PadType]()|Gamepad type setting|

#### Enums

##### __DragType__

|enums|description|
|:--|:--|
|NO_USE|Not used|
|MOVE|forward/backward movement|
|PAN|Left and right turning|
|SHIFT|up/down/left/right movement|

##### __PadType__

|enums|description|
|:--|:--|
|DEFAULT|standard controller|
|XBOXONE|XboxOne controller|

#### Example

- /Scenes/Examples/CameraControllExample.unity
