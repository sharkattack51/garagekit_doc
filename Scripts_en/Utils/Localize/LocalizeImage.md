# LocalizeImage

Image component with multi language switching support.

```csharp
namespace GarageKit.Localize
[ExecuteInEditMode]
public class LocalizeImage : MonoBehaviour, ILocalize
```

#### Inheritance

`LocalizeImage` -> `MonoBehaviour`, `ILocalize`

#### Inspector

<img src="~/image/script_reference/localizeimage_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiImage|Image|Image reference|
|localizeSprites|List<Sprite>|Sprite list for switching multi language|
|lang|[LANGUAGE](~/Scripts_en/Utils/Localize/Language.md)|Select language|

#### Static Methods

Multi language switching for all LocalizeImages
```csharp
public static void LocalizeAll(LANGUAGE lang)
```

#### Methods

Multi language switching
```csharp
public void Localize(LANGUAGE lang)
```
