# TimelineUtil

Provides utility functions related to Timeline operations.

> [!IMPORTANT]
> When using it, please enable #define definition in the source code.

```csharp
namespace GarageKit
public class TimelineUtil
```

#### Static Methods

Perform GC processing on management tracks
```csharp
public static void GavageManagedTracks()
```

Add track to timeline
```csharp
public static TrackAsset AddTrack<T>(PlayableDirector playableDirector, string trackName, UnityEngine.Object bindObj, TrackAsset parent = null) where T : TrackAsset
```

タイムラインからトラックを削除
```csharp
public static void DeleteTrack(PlayableDirector playableDirector, TrackAsset track)
```

Delete track from timeline
```csharp
public static void DeleteAllTrack(PlayableDirector playableDirector)
```

Delete a track from the timeline by specifying the track name
```csharp
public static void DeleteTrackByName(PlayableDirector playableDirector, string trackName)
```

Get by specifying track name
```csharp
public static TrackAsset GetTrackByName(PlayableDirector playableDirector, string trackName)
```

Get all tracks
```csharp
public static List<TrackAsset> GetAllTracks(PlayableDirector playableDirector)
```

Clear all clips by specifying track name
```csharp
public static void ClearTrackByName(PlayableDirector playableDirector, string trackName)
```

Clear all clips on all tracks
```csharp
public static void ClearAllTracks(PlayableDirector playableDirector)
```

Setting up a new track
```csharp
public static void SetTrack<T>(PlayableDirector playableDirector, string trackName, double start, double end) where T : TrackAsset
```

Setting up a new audio track
```csharp
public static void SetAudioTrack(PlayableDirector playableDirector, string trackName, AudioClip audioClip, double start, double? end = null, bool loop = false, double easeInDuration = 0.0, double easeOutDuration = 0.0)
```

Setting up a new RawImage track
```csharp
public static void SetRawImageTrack(PlayableDirector playableDirector, string trackName, Texture2D tex, double start, double end)
```

Setting up a new AVPro MediaPlayer track
```csharp
public static void SetMediaPlayerTrack(PlayableDirector playableDirector, string trackName, MediaPathType mediaPathType, string moviePath, double start, double? end = null)
public static void SetMediaPlayerTrack(PlayableDirector playableDirector, string trackName, double start, double? end = null, float vol = 1.0f)
```

Setting up a new activation track
```csharp
public static void SetActivationTrack(PlayableDirector playableDirector, string trackName, double start, double end)
```

Setting up a new animation track
```csharp
public static void SetAnimationTrack(PlayableDirector playableDirector, string trackName, AnimationClip animClip, double start, double end)
```

Setting up a new signal track
```csharp
public static void SetSignalTrack(PlayableDirector playableDirector, string trackName, SignalAsset signal, double time, string emitterName = "")
public static void SetSignalTrack(PlayableDirector playableDirector, SignalAsset signal, double time, string emitterName = "")
```

Get a list of each Clip In/Out time in a track
```csharp
public static List<Tuple<Double, Double>> GetClipsInOut(TrackAsset track)
```
