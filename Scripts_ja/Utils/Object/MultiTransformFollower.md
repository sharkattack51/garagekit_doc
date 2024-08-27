# MultiTransformFollower

Transform を複数のターゲットオブジェクト間と同期させます。[GizmoDrawer](~/Scripts_ja/Utils/Debug/GizmoDrawer.md) と一緒に利用すると便利です。

```csharp
namespace GarageKit
[ExecuteInEditMode]
public class MultiTransformFollower : MonoBehaviour
```

#### Inheritance

`MultiTransformFollower` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/multitransformfollower_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|target_A|GameObject|ターゲット A の参照|
|target_B|GameObject|ターゲット B の参照|
|lerp|float|2 ターゲット間同期の割合|
|followPosition|[MULTI_FOLLOW_AXIS](#multi_follow_axis)|位置の同期設定|
|followRotation|[MULTI_FOLLOW_AXIS](#multi_follow_axis)|回転の同期設定|
|followScale|[MULTI_FOLLOW_AXIS](#multi_follow_axis)|スケールの同期設定|

---

# MULTI_FOLLOW_AXIS

軸同期設定の構造体

```csharp
namespace GarageKit
[Serializable]
public class MULTI_FOLLOW_AXIS
```

#### Properties

|member|type|description|
|:--|:--|:--|
|x|bool|x 方向を有効化|
|y|bool|y 方向を有効化|
|z|bool|z 方向を有効化|
