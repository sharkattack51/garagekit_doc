# UIFadeTelop

CanvasGroup のフェード処理によるテキストを表示します。

```csharp
namespace GarageKit
public class UIFadeTelop : MonoBehaviour
```

#### Inheritance

`UIFadeTelop` -> [UIFadeGroupComponent](~/Scripts_ja/Utils/UI/UIFadeGroupComponent.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/uifadetelop_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiText|TMP_Text|テロップ用テキストの参照|
|uiTextBg|Image|背景イメージ|
|resizeBg|bool|背景をテキストサイズに合わせてリサイズする|

#### Methods

テロップのフェード表示開始
```csharp
public void StartTelop(string message, float fixTime = 5.0f, float tweenTime = 0.5f)
```
