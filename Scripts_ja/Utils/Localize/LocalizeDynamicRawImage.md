# LocalizeDynamicRawImage

多言語切り替え対応の RawImage コンポーネント

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
|uiRawImage|RawImage|RawImage の参照|
|localizeTexturePaths|List<string>|多言語切り替え用画像のパスリスト|
|lang|[LANGUAGE](~/Scripts_ja/Utils/Localize/Language.md)|選択言語|

#### Static Methods

全 LocalizeDynamicRawImage の非同期多言語切り替え
```csharp
public static async UniTask LocalizeAllAsync(LANGUAGE lang)
```

#### Methods

非同期多言語切り替え
```csharp
public async UniTask LocalizeAsync(LANGUAGE lang)
```

TryCatch による非同期多言語切り替え
```csharp
public async UniTask TryCatchLocalizeAsync(LANGUAGE lang, Action<Exception> onCatch, Action onFinally = null)
```
