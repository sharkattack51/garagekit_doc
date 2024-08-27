# SequenceTexture

フレームで連番 Texture を自動切り替えします。

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
|fps|int|切り替え FPS|
|isLoop|bool|ループ設定|
|textures|Texture2D[]|連番テクスチャリスト|
|textureParamName|string|テクスチャのセット先シェーダーパラメータ名|
