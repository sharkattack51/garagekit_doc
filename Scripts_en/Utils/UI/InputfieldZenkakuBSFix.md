# InputfieldZenkakuBSFix

A function to address the bug where the characters being converted double when the focus is removed from the InputField without finalizing it during full-width conversion of Japanese input.

reference: https://qiita.com/monolith8/items/a88b13ecc1121fa10450

```csharp
namespace GarageKit
[RequireComponent(typeof(InputField))]
public class InputfieldZenkakuBSFix : MonoBehaviour
```

#### Inheritance

`InputfieldZenkakuBSFix` -> `MonoBehaviour`
