# TextRandomizer

Runs an animation that randomly changes text.

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
|randomChars|string|Characters used for random text|
|uiText|TMP_Text|TMP_Text reference|

#### Methods

Start random text animation
```csharp
public void TextRandomizeIn(string goalText, float delay = 0.0f, int insertRndChrs = 10, bool defaultSalt = true)
```
