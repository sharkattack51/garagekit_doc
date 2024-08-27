# SoundManager

音声機能を管理します。再生に必要な AudioSource は内部で自動生成されて管理されます。

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
|soundLayers|List<[SoundLayerData](#soundlayerdata)>|サウンド設定|
|soundLayers3D|List<[Sound3DLayerData](#sound3dlayerdata)>|3D サウンド設定|
|SoundLayers|Dictionary<string, [SoundLayerData](#soundlayerdata)>|サウンド設定レイヤー名でのテーブル|
|SoundLayers3D|Dictionary<string, [Sound3DLayerData](#sound3dlayerdata)>|3D サウンド設定レイヤー名でのテーブル|
|masterMixerGroup|AudioMixerGroup|オプション: マスターミキサーグループ|
|decibelByStep|AnimationCurve|オプション: マスター音量のステップ調整用カーブ|

#### Methods

音声レイヤーの追加
```csharp
public void AddLayer(SoundLayerData layer)
```

音声レイヤーに音声クリップの追加
```csharp
public void AddClip(string layerName, string clipName, AudioClip clip)
```

音声の再生
```csharp
public void Play(string layerName, string clipName, bool overlap = false)
public void Play(string layerName, string clipName, bool overlap, bool loop, bool asOneShot)
```

音声レイヤーの再生状態確認
```csharp
public bool IsPlay(string layerName)
```

音声の再生停止
```csharp
public void Stop(string layerName = "")
```

全音声の再生停止
```csharp
public void StopAll(string layerName = "")
```

3D 音声レイヤーの追加
```csharp
public void AddLayer3D(Sound3DLayerData layer)
```

3D 音声レイヤーに 3D 音声ソースの追加
```csharp
public void AddSource3D(string layerName, string sourceName, AudioSource source)
```

3D 音声の再生
```csharp
public void Play3D(string layerName, string sourceName, bool overlap = false)
public void Play3D(string layerName, string sourceName, bool overlap, bool loop, bool asOneShot)
```

3D 音声レイヤーの再生状態確認
```csharp
public bool IsPlay3D(string layerName, string sourceName)
```

3D 音声の再生停止
```csharp
public void Stop3D(string layerName = "", string sourceName = "")
```

全 3D 音声の再生停止
```csharp
public void Stop3DAll(string layerName = "")
```

全音声のフェードイン
```csharp
public void FadeInAllSound(float time = 1.0f)
```

全音声のフェードアウト
```csharp
public void FadeOutAllSound(float time = 1.0f)
```

指定音声のフェード
```csharp
public void Fade(string layerName, float fromVol, float toVol, float time)
```

指定 3D 音声のフェード
```csharp
public void Fade3D(string layerName, string sourceName, float fromVol, float toVol, float time)
```

マスター音量ボリュームの設定
```csharp
public void SetMasterVol(float vol, string exposeProperty = "MasterVolume")
```

マスター音量ボリュームの1ステップアップ
```csharp
public void MasterVolUp(string exposeProperty = "MasterVolume")
```

マスター音量ボリュームの1ステップダウン
```csharp
public void MasterVolDown(string exposeProperty = "MasterVolume")
```

#### Example

```csharp
// 通常再生
AppMain.Instance.soundManager.Play("SE", "CLICK");

// オーバーラップ無しでループ再生
AppMain.Instance.soundManager.Play("BGM", "CLIP", false, true);
```

---

# SoundClipData

クリップ情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class SoundClipData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|clipName|string|クリップ名|
|clip|AudioClip|オーディオクリップ|

---

# SoundData

サウンド情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class SoundData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|use|bool|利用の有無|
|volume|float|音量ボリューム|
|clips|List<[SoundClipData](#soundclipdata)>|クリップ情報リスト|

---

# SoundLayerData

レイヤー情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class SoundLayerData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|layerName|string|レイヤー名|
|soundData|[SoundData](#sounddata)|サウンド情報|

#### Methods

レイヤーごとの処理の無効化設定
```csharp
public bool IgnoreAllMethod { get; set; }
```

---

# SoundSourceData

3D サウンドソース情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class SoundSourceData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|sourceName|string|3D サウンドソース名|
|source|AudioSource|オーディオソース|

---

# Sound3DData

3D サウンド情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class Sound3DData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|use|bool|利用の有無|
|volume|float|音量ボリューム|
|sources|List<[SoundSourceData](#soundsourcedata)>|3D サウンドソース情報リスト|

---

# Sound3DLayerData

3D レイヤー情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class Sound3DLayerData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|layerName|string|レイヤー名|
|soundData|[Sound3DData](#sound3ddata)|サウンド情報|

#### Methods

レイヤーごとの処理の無効化設定
```csharp
public bool IgnoreAllMethod { get; set; }
```
