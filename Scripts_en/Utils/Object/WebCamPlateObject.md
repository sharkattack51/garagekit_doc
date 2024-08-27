# WebCamPlateObject

Simplifies settings when using a web camera. The image is reflected in the texture.

```csharp
namespace GarageKit
[RequireComponent(typeof(Renderer))]
public class WebCamPlateObject : MonoBehaviour
```

#### Inheritance

`WebCamPlateObject` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/webcamplateobject_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|deviceName|string|Specifying camera device name|
|deviceIndex|int|Specifying camera device id|
|requestedWidth|int|Camera image width specification|
|requestedHeight|int|Camera image hejght specification|
|requestedFPS|int|Camera image FPS specification|
|anisoLevel|int|Anisotropic filtering level of texture|
|texturePropName|string|Shader texture property name|
|filteMode|FilterMode|Filter mode of texture|
|wrapMode|TextureWrapMode|Wrap mode of texture|
|isAutoAspect|bool|Automatic aspect setting|
|isMirror|bool|Horizontal flip setting|
|isMobileCameraRotation|bool|Reflecting the rotation direction of the device|
|vertical|[OBJECTAXIS_Y](#objectaxis_y)|Upward axis setting|

#### Enums

##### __OBJECTAXIS_Y__

|enums|description|
|:--|:--|
|Y|Object Y axis direction|
|Z|Object Z axis direction|

#### Methods

Get WebCamTexture
```csharp
public WebCamTexture WebCamTexture { get; }
```

Check if the webcam is open
```csharp
public bool IsWebCamPlaySuccess()
```
