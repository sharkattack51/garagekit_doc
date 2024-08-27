# Fader

Set it on the camera and perform the fade using GL drawing processing. Drawn at the end of all drawings. It is automatically set when using [AsyncStateBase](~/Scripts_en/Utils/State/Base/AsyncStateBase.md).

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
|fadeTime|float|Fade time|
|fadeColor|Color|Fade color|
|fadeMaterial|Material|Fade material|
|fadeType|[FADE_TYPE](#fade_type)|Fade type|

#### Enums

##### __FADE_TYPE__

|enums|description|
|:--|:--|
|FADE_IN|Fade in|
|FADE_OUT|Fade out|

#### Static Methods

Enabling/disabling fade
```csharp
public static bool UseFade { get; }
```

List of all Fader components in the scene
```csharp
public static List<Fader> Faders { get; }
```

Start fading all Fader components
```csharp
public static void StartFadeAll(FADE_TYPE fadeType)
public static void StartFadeAll(float fadeTime, FADE_TYPE fadeType)
```

#### Methods

Checking if it's fading
```csharp
public bool IsFading { get; }
```

Enabling fade
```csharp
public static void EnableFade()
```

Disabling fade
```csharp
public static void DisableFade()
```

Start fade
```csharp
public void StartFade(FADE_TYPE fadeType, float targetAlpha = 1.0f)
public void StartFade(float fadeTime, FADE_TYPE fadeType, float targetAlpha = 1.0f)
```
