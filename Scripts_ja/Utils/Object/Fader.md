# Fader

カメラに設定して GL 描画処理でフェードを行います。全描画の最後に描画されます。[AsyncStateBase](~/Scripts_ja/Utils/State/Base/AsyncStateBase.md) を利用する場合は自動的に設定されます。

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class Fader : MonoBehaviour
```

#### Inheritance

`Fader` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/fader_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|fadeTime|float|フェード時間|
|fadeColor|Color|フェードカラー|
|fadeMaterial|Material|描画用マテリアル|
|fadeType|[FADE_TYPE](#fade_type)|フェードタイプ|

#### Enums

##### __FADE_TYPE__

|enums|description|
|:--|:--|
|FADE_IN|フェードイン|
|FADE_OUT|フェードアウト|

#### Static Methods

フェードの有効無効
```csharp
public static bool UseFade { get; }
```

シーン内の全 Fader コンポーネントリスト
```csharp
public static List<Fader> Faders { get; }
```

全 Fader コンポーネントのフェードを開始
```csharp
public static void StartFadeAll(FADE_TYPE fadeType)
public static void StartFadeAll(float fadeTime, FADE_TYPE fadeType)
```

#### Methods

フェード中確認
```csharp
public bool IsFading { get; }
```

フェードの有効化
```csharp
public static void EnableFade()
```

フェードの無効化
```csharp
public static void DisableFade()
```

フェードを開始
```csharp
public void StartFade(FADE_TYPE fadeType, float targetAlpha = 1.0f)
public void StartFade(float fadeTime, FADE_TYPE fadeType, float targetAlpha = 1.0f)
```
