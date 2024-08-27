# TextRandomizer

テキストをランダムに変更するアニメーションを実行します。

```csharp
namespace GarageKit
public class TextRandomizer : MonoBehaviour
```

#### Inheritance

`TextRandomizer` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/textrandomizer_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|randomChars|string|ランダムテキストに利用するキャラクター|
|uiText|TMP_Text|TMP_Text の参照|

#### Methods

テキストのランダムアニメーションを開始
```csharp
public void TextRandomizeIn(string goalText, float delay = 0.0f, int insertRndChrs = 10, bool defaultSalt = true)
```
