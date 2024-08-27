# UIMovieControllPanel

Provides control panel functionality for movie playback using [AVProVideo](https://assetstore.unity.com/packages/tools/video/avpro-video-v3-ultra-edition-278896).

> [!IMPORTANT]
> Requires the [AVProVideo](https://assetstore.unity.com/packages/tools/video/avpro-video-v3-ultra-edition-278896) package. When using it, please enable #define definition in the source code.

> [!IMPORTANT]
> Available from configured prefabs within the package. Add DisplayUGUI and TMP_Text components in the prefab and reset each reference to use them.

```csharp
namespace GarageKit
public class UIMovieControllPanel : MonoBehaviour
```

#### Inheritance

`ARTrackedImageMarkerManager` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/uimoviecontrollpanel_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|player|MediaPlayer|MediaPlayer reference|
|setupOnStart|bool|Set up with Start()|
|uiMovie|DisplayUGUI|DisplayUGUI reference|
|uiPlayPauseBtn|Button|Play/Pause button reference|
|uiSeekSlider|Slider|Seek slider reference|
|uiElapsedTxt|TMP_Text|Remaining time TMP_Text reference|
|seekEventTrg|EventTrigger|EventTrigger reference for seek event|
|playSprite|Sprite|Play button Sprite|
|pauseSprite|Sprite|Pause button Sprite|

#### Methods

Callback when playback start
```csharp
public Action OnPlay
```

Callback when paused
```csharp
public Action OnPause
```

Callback when seek start
```csharp
public Action<float> OnSeekStart
```

Callback when seeking
```csharp
public Action<float> OnSeek
```

Callback when seek end
```csharp
public Action<float> OnSeekEnd
```

Callback when playback complete
```csharp
public Action OnFinishedPlaying
```

Clear movie
```csharp
public void Clear()
```

Setup this controll panel
```csharp
public void Setup()
```

Load movie
```csharp
public bool Load(string moviePathOrUrl, MediaPathType pathType = MediaPathType.AbsolutePathOrURL, bool autoPlay = false)
```

#### Example

- \_\_ProjectName\_\_/Prefabs/Utils/UI/MovieControllPanel.prefab

```csharp
// Setup required before loading and playing
uiMovieControllPanel.Setup();
uiMovieControllPanel.Load("test.mp4");
```
