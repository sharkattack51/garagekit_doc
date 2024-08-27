# TransformFollower

Synchronize the Transform with the target object. It is useful to use it together with [GizmoDrawer](~/Scripts_en/Utils/Debug/GizmoDrawer.md).

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
|targetObject|GameObject|Target reference|
|followPosition|[FOLLOW_AXIS](#follow_axis)|Position sync setting|
|followRotation|[FOLLOW_AXIS](#follow_axis)|Rotation sync setting|
|followScale|[FOLLOW_AXIS](#follow_axis)|Scale sync setting|

---

# FOLLOW_AXIS

Sync axis information structure

```csharp
namespace GarageKit
[Serializable]
public class FOLLOW_AXIS
```

#### Properties

|member|type|description|
|:--|:--|:--|
|x|bool|Enable x direction|
|y|bool|Enable y direction|
|z|bool|Enable z direction|
