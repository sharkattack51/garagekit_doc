# NumberTexture

入力された 0-9 の数値からテクスチャを設定して切り替えます。

```csharp
namespace GarageKit
public class NumberTexture : MonoBehaviour
```

#### Inheritance

`NumberTexture` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/numberexture_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|numTextures|Texture2D[]|数字テクスチャ 0-9|
|numPlates|GameObject[]|一の位を先頭にする桁オブジェクト|

#### Methods

番号テクスチャの設定
```csharp
public void SetNumber(int num)
```
