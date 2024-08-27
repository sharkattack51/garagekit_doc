# MultiTransformFollower

Synchronize Transforms between multiple target objects. It is useful to use it together with [GizmoDrawer](~/Scripts_en/Utils/Debug/GizmoDrawer.md).

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
|target_A|GameObject|Target A reference|
|target_B|GameObject|Target B reference|
|lerp|float|Position between two targets|
|followPosition|[MULTI_FOLLOW_AXIS](#multi_follow_axis)|Position sync setting|
|followRotation|[MULTI_FOLLOW_AXIS](#multi_follow_axis)|Rotation sync setting|
|followScale|[MULTI_FOLLOW_AXIS](#multi_follow_axis)|Scale sync setting|

---

# MULTI_FOLLOW_AXIS

Sync axis information structure

```csharp
namespace GarageKit
[Serializable]
public class MULTI_FOLLOW_AXIS
```

#### Properties

|member|type|description|
|:--|:--|:--|
|x|bool|Enable x direction|
|y|bool|Enable y direction|
|z|bool|Enable z direction|
