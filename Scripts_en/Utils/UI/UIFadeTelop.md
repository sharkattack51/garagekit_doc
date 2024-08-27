# UIFadeTelop

Displays faded text in a CanvasGroup.

```csharp
namespace GarageKit
public class UIFadeTelop : MonoBehaviour
```

#### Inheritance

`UIFadeTelop` -> [UIFadeGroupComponent](~/Scripts_en/Utils/UI/UIFadeGroupComponent.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/uifadetelop_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiText|TMP_Text|TMP_Text reference|
|uiTextBg|Image|Background image|
|resizeBg|bool|Resize the background to fit the text size|

#### Methods

Start of fading of captions
```csharp
public void StartTelop(string message, float fixTime = 5.0f, float tweenTime = 0.5f)
```
