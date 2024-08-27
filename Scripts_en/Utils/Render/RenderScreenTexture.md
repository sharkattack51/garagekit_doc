# RenderScreenTexture

Set RenderTexture on the camera so that it can be obtained externally.

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class RenderScreenTexture : MonoBehaviour
```

#### Inheritance

`RenderScreenTexture` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/renderscreentexture_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|asScreenSize|bool|Automatic setting by screen size|
|textureSize|Vector2|RenderTexture size|

#### Methods

Get screen RenderTexture
```csharp
public RenderTexture GetRenderTexture()
```
