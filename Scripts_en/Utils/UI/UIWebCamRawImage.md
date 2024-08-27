# UIWebCamRawImage

Simplifies uGUI RawImage settings that use a web camera.

```csharp
namespace GarageKit
[RequireComponent(typeof(RawImage))]
public class UIWebCamRawImage : MonoBehaviour
```

#### Inheritance

`UIWebCamRawImage` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/webcamrawimage_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|webcamPlayOnStart|bool|Start playback with Start()|
|deviceName|string|Specifying camera device name|
|deviceIndex|int|Specifying camera device id|
|requestedWidth|int|Camera image width specification|
|requestedHeight|int|Camera image height specification|
|requestedFPS|int|Camera image FPS specification|
|anisoLevel|int|Anisotropic filtering level of texture|
|filteMode|FilterMode|Filter mode of texture|
|wrapMode|TextureWrapMode|Wrap mode of texture|
|isAutoScreenAspect|bool|Automatic aspect setting|
|isMirror|bool|Horizontal flip setting|
|appOrientation|[APP_ORIENTATION](#app_orientation)|Screen orientation|

#### Enums

##### __APP_ORIENTATION__

|enums|description|
|:--|:--|
|PORTRAIT|Device vertical position|
|LANDSCAPE|Device horizontal position|

#### Methods

Get WebCamTexture
```csharp
public WebCamTexture WebCamTexture { get; }
```

Start webcam
```csharp
public IEnumerator WebcamPlay()
```

Stop webcam
```csharp
public void WebcamStop()
```

Check if the webcam is open
```csharp
public bool IsWebcamPlay()
```
