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
|isMirror|bool|Horizontal flip setting|
|appOrientation|[APP_ORIENTATION](#app_orientation)|Screen orientation|
|aspectFitMode|[ASPECT_FIT_MODE](#aspect_fit_mode)|Aspect ratio settings|

#### Enums

##### __APP_ORIENTATION__

|enums|description|
|:--|:--|
|PORTRAIT|Device vertical position|
|LANDSCAPE|Device horizontal position|
|LANDSCAPE_LEFT|Device horizontal position(home button on the left)|

##### __ASPECT_FIT_MODE__

|enums|description|
|:--|:--|
|NONE|無し|
|FIT_WIDTH|Fit width|
|FIT_HEIGHT|Fit height|

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
