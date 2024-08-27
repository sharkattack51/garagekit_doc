# LocalizeImage

多言語切り替え対応の Image コンポーネント

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
|uiImage|Image|Image の参照|
|localizeSprites|List<Sprite>|多言語切り替え用スプライトリスト|
|lang|[LANGUAGE](~/Scripts_ja/Utils/Localize/Language.md)|選択言語|

#### Static Methods

全 LocalizeImage の多言語切り替え
```csharp
public static void LocalizeAll(LANGUAGE lang)
```

#### Methods

多言語切り替え
```csharp
public void Localize(LANGUAGE lang)
```
