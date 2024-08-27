# C4DAnimDataApply

Cinema4D から書き出されたアニメーションキーフレームデータ（.json）をアニメーションカーブに変換します。

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
|filePath|string|読み込み json ファイルパス|
|animTracks|[C4DAnimationTrack](#c4danimationtrack)[]|Cinema4D アニメーショントラックリスト|

#### Methods

変換アニメーションデータテーブルの取得
```csharp
public Dictionary<string, List<float>> Data { get; }
```

アニメーションカーブの取得
```csharp
public AnimationCurve GetCurve(C4DAnimationTrack.TRACK_TYPE type)
```

アニメーションフレーム数の取得
```csharp
public int GetTotalFrame()
```

---

# C4DAnimationTrack

Cinema4D アニメーショントラックデータの構造体

```csharp
namespace GarageKit
[Serializable]
public class C4DAnimationTrack
```

#### Properties

|member|type|description|
|:--|:--|:--|
|type|[TRACK_TYPE](#track_type)|アニメーショントラックタイプ|
|curve|AnimationCurve|読み込みデータから変換生成されるアニメーションカーブ|

#### Enums

##### __TRACK_TYPE__

|enums|description|
|:--|:--|
|POS_X|X 位置トラック|
|POS_Y|Y 位置トラック|
|POS_Z|Z 位置トラック|
|ROT_X|X 回転トラック|
|ROT_Y|Y 回転トラック|
|ROT_Z|Z 回転トラック|

#### Methods

トラック名の取得
```csharp
public string GetTrackName()
```