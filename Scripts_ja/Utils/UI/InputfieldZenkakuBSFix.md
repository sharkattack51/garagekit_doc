# InputfieldZenkakuBSFix

日本語入力の全角変換中に確定させない状態で InputField からフォーカスを外すと変換中の文字が倍加するバグの対応機能

reference: https://qiita.com/monolith8/items/a88b13ecc1121fa10450

```csharp
namespace GarageKit
[RequireComponent(typeof(InputField))]
public class InputfieldZenkakuBSFix : MonoBehaviour
```

#### Inheritance

`InputfieldZenkakuBSFix` -> `MonoBehaviour`
