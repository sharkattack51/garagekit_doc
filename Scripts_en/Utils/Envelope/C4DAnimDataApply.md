# C4DAnimDataApply

Converts animation keyframe data (.json) exported from Cinema4D to animation curves.

```csharp
namespace GarageKit
public class C4DAnimDataApply : MonoBehaviour
```

#### Inheritance

`C4DAnimDataApply` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/c4danimdataapply_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|filePath|string|Load json file path|
|animTracks|[C4DAnimationTrack](#c4danimationtrack)[]|Cinema4D animation track list|

#### Methods

Get converted animation data table
```csharp
public Dictionary<string, List<float>> Data { get; }
```

Get animation curve
```csharp
public AnimationCurve GetCurve(C4DAnimationTrack.TRACK_TYPE type)
```

Get animation length
```csharp
public int GetTotalFrame()
```

---

# C4DAnimationTrack

Cinema4D animation track data structure

```csharp
namespace GarageKit
[Serializable]
public class C4DAnimationTrack
```

#### Properties

|member|type|description|
|:--|:--|:--|
|type|[TRACK_TYPE](#track_type)|Animation track type|
|curve|AnimationCurve|Animation curve generated from conversion from loaded data|

#### Enums

##### __TRACK_TYPE__

|enums|description|
|:--|:--|
|POS_X|X position track|
|POS_Y|Y position track|
|POS_Z|Z position track|
|ROT_X|X axis rotation track|
|ROT_Y|Y axis rotation track||
|ROT_Z|Z axis rotation track||

#### Methods

Get track name
```csharp
public string GetTrackName()
```