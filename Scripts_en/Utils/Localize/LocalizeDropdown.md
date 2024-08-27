# LocalizeDropdown

TMP_Dropdown component with multi language switching support.

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
|uiDropdown|TMP_Dropdown|TMP_Dropdown reference|
|localizeFonts|List<TMP_FontAsset>|Font list for switching multi language|
|localizeDropdownStrings|List<[LocalizeDropdownStrings](#localizedropdownstrings)>|List of text in dropdown to switching multi language|

#### Static Methods

Multi language switching for all LocalizeDropdowns
```csharp
public static void LocalizeAll(LANGUAGE lang)
```

#### Methods

Multi language switching
```csharp
public void Localize(LANGUAGE lang)
```

---

# LocalizeDropdownStrings

Structure of text list data in dropdown for switching multi language

```csharp
namespace GarageKit.Localize
[Serializable]
public class LocalizeDropdownStrings
```

#### Properties

|member|type|description|
|:--|:--|:--|
|localizeStrings|List<string>|Text in each language|
