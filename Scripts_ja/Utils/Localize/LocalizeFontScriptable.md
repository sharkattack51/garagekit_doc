# LocalizeFontScriptable

多言語切り替え用フォント設定のシリアライズ ScriptableObject

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
|localizeFonts|List<[LocalizeFont](#localizefont)>|多言語切り替えフォント設定のリスト|

---

# LocalizeFont

多言語切り替えフォント設定の構造体

```csharp
namespace GarageKit.Localize
[Serializable]
public class LocalizeFont
```

#### Properties

|member|type|description|
|:--|:--|:--|
|lang|LANGUAGE|選択言語|
|font|TMP_FontAsset|フォント|
