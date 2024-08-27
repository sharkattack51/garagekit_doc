# LocalizeDropdown

多言語切り替え対応の TMP_Dropdown コンポーネント

```csharp
namespace GarageKit.Localize
public class LocalizeDropdown : MonoBehaviour, ILocalize
```

#### Inheritance

`LocalizeDropdown` -> `MonoBehaviour`, `ILocalize`

#### Inspector

<img src="~/image/script_reference/localizedropdown_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiDropdown|TMP_Dropdown|TMP_Dropdown の参照|
|localizeFonts|List<TMP_FontAsset>|多言語切り替え用フォントリスト|
|localizeDropdownStrings|List<[LocalizeDropdownStrings](#localizedropdownstrings)>|多言語切り替え用ドロップダウン内テキストリスト|

#### Static Methods

全 LocalizeDropdown の多言語切り替え
```csharp
public static void LocalizeAll(LANGUAGE lang)
```

#### Methods

多言語切り替え
```csharp
public void Localize(LANGUAGE lang)
```

---

# LocalizeDropdownStrings

多言語切り替え用ドロップダウン内テキストリストデータの構造体

```csharp
namespace GarageKit.Localize
[Serializable]
public class LocalizeDropdownStrings
```

#### Properties

|member|type|description|
|:--|:--|:--|
|localizeStrings|List<string>|各言語テキスト|
