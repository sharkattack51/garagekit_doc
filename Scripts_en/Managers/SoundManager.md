# SoundManager

Manage sound features. The AudioSource required for playback is automatically generated and managed internally.

```csharp
namespace GarageKit
public class SoundManager : ManagerBase
```

#### Inheritance

`SoundManager` -> [ManagerBase](../Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/soundmanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|soundLayers|List<[SoundLayerData](#soundlayerdata)>|Sound setting|
|soundLayers3D|List<[Sound3DLayerData](#sound3dlayerdata)>|3D Sound setting|
|SoundLayers|Dictionary<string, [SoundLayerData](#soundlayerdata)>|Table with sound layer names|
|SoundLayers3D|Dictionary<string, [Sound3DLayerData](#sound3dlayerdata)>|Table with 3D sound layer names|
|masterMixerGroup|AudioMixerGroup|Option: Master mixer group|
|decibelByStep|AnimationCurve|Option: Master volume step adjustment curve|

#### Methods

Add sound layer
```csharp
public void AddLayer(SoundLayerData layer)
```

Add AudioClip to sound layer
```csharp
public void AddClip(string layerName, string clipName, AudioClip clip)
```

Sound playback
```csharp
public void Play(string layerName, string clipName, bool overlap = false)
public void Play(string layerName, string clipName, bool overlap, bool loop, bool asOneShot)
```

Playback status of the sound layer
```csharp
public bool IsPlay(string layerName)
```

Stop sound playback
```csharp
public void Stop(string layerName = "")
```

Stop playing all sounds
```csharp
public void StopAll(string layerName = "")
```

Add 3D sound layer
```csharp
public void AddLayer3D(Sound3DLayerData layer)
```

3D 音声レイヤーに 3D 音声ソースの追加
Add 3D AudioSource to 3D sound layer
```csharp
public void AddSource3D(string layerName, string sourceName, AudioSource source)
```

3D sound playback
```csharp
public void Play3D(string layerName, string sourceName, bool overlap = false)
public void Play3D(string layerName, string sourceName, bool overlap, bool loop, bool asOneShot)
```

Playback status of the 3D sound layer
```csharp
public bool IsPlay3D(string layerName, string sourceName)
```

Stop 3D sound playback
```csharp
public void Stop3D(string layerName = "", string sourceName = "")
```

Stop playing all 3D sounds
```csharp
public void Stop3DAll(string layerName = "")
```

Fade in all sounds
```csharp
public void FadeInAllSound(float time = 1.0f)
```

Fade out all sounds
```csharp
public void FadeOutAllSound(float time = 1.0f)
```

Fade of specified sound
```csharp
public void Fade(string layerName, float fromVol, float toVol, float time)
```

Fade of specified 3D sound
```csharp
public void Fade3D(string layerName, string sourceName, float fromVol, float toVol, float time)
```

Setting the master volume
```csharp
public void SetMasterVol(float vol, string exposeProperty = "MasterVolume")
```

Master volume step up one
```csharp
public void MasterVolUp(string exposeProperty = "MasterVolume")
```

Master volume step down one
```csharp
public void MasterVolDown(string exposeProperty = "MasterVolume")
```

#### Example

```csharp
// Normal playback
AppMain.Instance.soundManager.Play("SE", "CLICK");

// Loop playback without overlap
AppMain.Instance.soundManager.Play("BGM", "CLIP", false, true);
```

---

# SoundClipData

Clip information structure

```csharp
namespace GarageKit
[Serializable]
public class SoundClipData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|clipName|string|Clip name|
|clip|AudioClip|AudioClip reference|

---

# SoundData

Sound information structure

```csharp
namespace GarageKit
[Serializable]
public class SoundData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|use|bool|Use it or not|
|volume|float|Sound volume|
|clips|List<[SoundClipData](#soundclipdata)>|Clip information list|

---

# SoundLayerData

Layer information structure

```csharp
namespace GarageKit
[Serializable]
public class SoundLayerData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|layerName|string|Layer name|
|soundData|[SoundData](#sounddata)|Sound information|

#### Methods

Disable processing for each layer
```csharp
public bool IgnoreAllMethod { get; set; }
```

---

# SoundSourceData

3D sound source information structure

```csharp
namespace GarageKit
[Serializable]
public class SoundSourceData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|sourceName|string|3D sound source name|
|source|AudioSource|AudioSource reference|

---

# Sound3DData

3D sound information structure

```csharp
namespace GarageKit
[Serializable]
public class Sound3DData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|use|bool|Use it or not|
|volume|float|SOund volume|
|sources|List<[SoundSourceData](#soundsourcedata)>|3D sound source information list|

---

# Sound3DLayerData

3D layer information structure

```csharp
namespace GarageKit
[Serializable]
public class Sound3DLayerData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|layerName|string|Layer name|
|soundData|[Sound3DData](#sound3ddata)|Sound information|

#### Methods

Disable processing for each layer
```csharp
public bool IgnoreAllMethod { get; set; }
```
