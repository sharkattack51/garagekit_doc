# LocalizeText

TMP_Text component with multi language switching support.

```csharp
namespace GarageKit.Localize
[ExecuteInEditMode]
public class LocalizeText : MonoBehaviour, ILocalize
```

#### Inheritance

`LocalizeText` -> `MonoBehaviour`, `ILocalize`

#### Inspector

<img src="~/image/script_reference/localizetext_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiText|TMP_Text|TMP_Text reference|
|localizeFonts|List<TMP_FontAsset>|Font list for switching multi language|
|lalocalizeFontScriptableng|[LocalizeFontScriptable](~/Scripts_en/Utils/Localize/LocalizeFontScriptable.md)|Serialized multi language switching font settings. supersedes localizeFonts|
|localizeStrings|List<string>|Text list for switching multi language|
|lang|[LANGUAGE](~/Scripts_en/Utils/Localize/Language.md)|Select language|

#### Static Methods

Multi language switching for all LocalizeText
```csharp
public static void LocalizeAll(LANGUAGE lang)
```

#### Methods

Multi language switching
```csharp
public void Localize(LANGUAGE lang)
```
