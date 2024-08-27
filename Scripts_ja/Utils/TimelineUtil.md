# TimelineUtil

Timeline操作関連のユーティリティ関数を提供します。

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
public class TimelineUtil
```

#### Static Methods

管理トラックの GC 処理を行う
```csharp
public static void GavageManagedTracks()
```

タイムラインにトラックを追加
```csharp
public static TrackAsset AddTrack<T>(PlayableDirector playableDirector, string trackName, UnityEngine.Object bindObj, TrackAsset parent = null) where T : TrackAsset
```

タイムラインからトラックを削除
```csharp
public static void DeleteTrack(PlayableDirector playableDirector, TrackAsset track)
```

タイムラインから全トラックを削除
```csharp
public static void DeleteAllTrack(PlayableDirector playableDirector)
```

トラック名を指定してタイムラインからトラックを削除
```csharp
public static void DeleteTrackByName(PlayableDirector playableDirector, string trackName)
```

トラック名を指定して取得
```csharp
public static TrackAsset GetTrackByName(PlayableDirector playableDirector, string trackName)
```

全トラックを取得
```csharp
public static List<TrackAsset> GetAllTracks(PlayableDirector playableDirector)
```

トラック名を指定して全クリップをクリア
```csharp
public static void ClearTrackByName(PlayableDirector playableDirector, string trackName)
```

全トラックの全クリップをクリア
```csharp
public static void ClearAllTracks(PlayableDirector playableDirector)
```

新規トラックの設定
```csharp
public static void SetTrack<T>(PlayableDirector playableDirector, string trackName, double start, double end) where T : TrackAsset
```

新規音声トラックの設定
```csharp
public static void SetAudioTrack(PlayableDirector playableDirector, string trackName, AudioClip audioClip, double start, double? end = null, bool loop = false, double easeInDuration = 0.0, double easeOutDuration = 0.0)
```

新規 RawImage トラックの設定
```csharp
public static void SetRawImageTrack(PlayableDirector playableDirector, string trackName, Texture2D tex, double start, double end)
```

新規 AVPro MediaPlayer トラックの設定
```csharp
public static void SetMediaPlayerTrack(PlayableDirector playableDirector, string trackName, MediaPathType mediaPathType, string moviePath, double start, double? end = null)
public static void SetMediaPlayerTrack(PlayableDirector playableDirector, string trackName, double start, double? end = null, float vol = 1.0f)
```

新規アクティベーショントラックの設定
```csharp
public static void SetActivationTrack(PlayableDirector playableDirector, string trackName, double start, double end)
```

新規アニメーショントラックの設定
```csharp
public static void SetAnimationTrack(PlayableDirector playableDirector, string trackName, AnimationClip animClip, double start, double end)
```

新規シグナルトラックの設定
```csharp
public static void SetSignalTrack(PlayableDirector playableDirector, string trackName, SignalAsset signal, double time, string emitterName = "")
public static void SetSignalTrack(PlayableDirector playableDirector, SignalAsset signal, double time, string emitterName = "")
```

トラック内の各 Clip In/Out 時間リストの取得
```csharp
public static List<Tuple<Double, Double>> GetClipsInOut(TrackAsset track)
```
