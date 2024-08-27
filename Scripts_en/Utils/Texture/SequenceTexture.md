# SequenceTexture

Automatically switch sequential number Texture in frame.

```csharp
namespace GarageKit
public class SequenceTexture : MonoBehaviour
```

#### Inheritance

`SequenceTexture` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/sequencestexture_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|fps|int|Switching FPS|
|isLoop|bool|Loop settings|
|textures|Texture2D[]|Sequential texture list|
|textureParamName|string|Shader parameter name where texture is set|
