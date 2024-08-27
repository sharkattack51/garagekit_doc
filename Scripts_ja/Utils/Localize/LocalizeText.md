# LocalizeText

多言語切り替え対応の TMP_Text コンポーネント

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
|uiText|TMP_Text|TMP_Text の参照|
|localizeFonts|List<TMP_FontAsset>|多言語切り替え用フォントリスト|
|lalocalizeFontScriptableng|[LocalizeFontScriptable](~/Scripts_ja/Utils/Localize/LocalizeFontScriptable.md)|シリアライズされている多言語切り替え用フォント設定 localizeFonts よりも優先|
|localizeStrings|List<string>|多言語切り替え用テキストリスト|
|lang|[LANGUAGE](~/Scripts_ja/Utils/Localize/Language.md)|選択言語|

#### Static Methods

全 LocalizeText の多言語切り替え
```csharp
public static void LocalizeAll(LANGUAGE lang)
```

#### Methods

多言語切り替え
```csharp
public void Localize(LANGUAGE lang)
```
