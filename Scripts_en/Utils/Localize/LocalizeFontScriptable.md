# LocalizeFontScriptable

​​ScriptableObject for serializing font settings for switching multi language.

```csharp
namespace GarageKit.Localize
[CreateAssetMenu(menuName = "GarageKit/Localize Font Asset", fileName = "LocalizeFontAsset")]
public class LocalizeFontScriptable : ScriptableObject
```

#### Inheritance

`LocalizeFontScriptable` -> `ScriptableObject`

#### Inspector

<img src="~/image/script_reference/localizefontscriptable_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|localizeFonts|List<[LocalizeFont](#localizefont)>|List of multi language switching font settings|

---

# LocalizeFont

Structure of multi language switching font settings

```csharp
namespace GarageKit.Localize
[Serializable]
public class LocalizeFont
```

#### Properties

|member|type|description|
|:--|:--|:--|
|lang|LANGUAGE|Set language|
|font|TMP_FontAsset|Font data|
