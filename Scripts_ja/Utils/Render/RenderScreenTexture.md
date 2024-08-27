# RenderScreenTexture

カメラに RenderTexture を設定して外部から取得可能にします。

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
|asScreenSize|bool|スクリーンサイズでの自動設定|
|textureSize|Vector2|RenderTexture サイズ|

#### Methods

RenderTexture の取得
```csharp
public RenderTexture GetRenderTexture()
```
