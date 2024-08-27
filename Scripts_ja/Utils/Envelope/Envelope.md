# Envelope

キーフレームデータリストから実行時動的にアニメーションカーブを作成します。

```csharp
namespace GarageKit
public class Envelope : MonoBehaviour
```

#### Inheritance

`Envelope` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/envelope_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|propertyName|string|識別用プロパティ名|
|preWrapMode|WrapMode|前方向のラップモード|
|postWrapMode|WrapMode|後方向のラップモード|
|envelopeKeys|[EnvelopeKey](#envelopekey)[]|キーフレームデータリスト|

#### Methods

アニメーションカーブの取得
```csharp
public AnimationCurve GetCurve()
```

---

# EnvelopeKey

キーフレームデータの構造体

```csharp
namespace GarageKit
[Serializable]
public class EnvelopeKey
```

#### Properties

|member|type|description|
|:--|:--|:--|
|time|float|時間 X|
|value|float|値 Y|
|leftTangent|AnimationCurveUtil.TangentMode|左ハンドルタンジェント|
|rightTangent|AnimationCurveUtil.TangentMode|右ハンドルタンジェント|
