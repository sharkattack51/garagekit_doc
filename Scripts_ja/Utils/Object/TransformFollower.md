# TransformFollower

Transform をターゲットオブジェクトと同期させます。[GizmoDrawer](~/Scripts_ja/Utils/Debug/GizmoDrawer.md) と一緒に利用すると便利です。

```csharp
namespace GarageKit
[ExecuteInEditMode]
public class TransformFollower : MonoBehaviour
```

#### Inheritance

`TransformFollower` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/transformfollower_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|targetObject|GameObject|ターゲットの参照|
|followPosition|[FOLLOW_AXIS](#follow_axis)|位置の同期設定|
|followRotation|[FOLLOW_AXIS](#follow_axis)|回転の同期設定|
|followScale|[FOLLOW_AXIS](#follow_axis)|スケールの同期設定|

---

# FOLLOW_AXIS

軸同期設定の構造体

```csharp
namespace GarageKit
[Serializable]
public class FOLLOW_AXIS
```

#### Properties

|member|type|description|
|:--|:--|:--|
|x|bool|x 方向を有効化|
|y|bool|y 方向を有効化|
|z|bool|z 方向を有効化|
