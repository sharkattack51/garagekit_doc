# LocalizeDynamicRawImage

RawImage component with multi　language switching support.

```csharp
namespace GarageKit.Localize
public class LocalizeDynamicRawImage : MonoBehaviour, ILocalize
```

#### Inheritance

`LocalizeDynamicRawImage` -> `MonoBehaviour`, `ILocalize`

#### Inspector

<img src="~/image/script_reference/localizedynamicrawimage_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiRawImage|RawImage|RawImage reference|
|localizeTexturePaths|List<string>|Image path list for switching multi language|
|lang|[LANGUAGE](~/Scripts_en/Utils/Localize/Language.md)|select language|

#### Static Methods

Asynchronous multi language switching for all LocalizeDynamicRawImages.
```csharp
public static async UniTask LocalizeAllAsync(LANGUAGE lang)
```

#### Methods

Asynchronous multi language switching
```csharp
public async UniTask LocalizeAsync(LANGUAGE lang)
```

Asynchronous multi language switching with TryCatch
```csharp
public async UniTask TryCatchLocalizeAsync(LANGUAGE lang, Action<Exception> onCatch, Action onFinally = null)
```
