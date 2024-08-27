# GizmoDrawer

Displays the gizmo in SceneView even when no object is selected.

<img src="~/image/script_reference/gizmodrawer_sceneview.png" width="500px"/>
</br>
</br>

```csharp
namespace GarageKit
public class GizmoDrawer : MonoBehaviour
```

#### Inheritance

`GizmoDrawer` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/gizmodrawer_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|gizmoType|[GIZMO_TYPE](#gizmo_type)|Gizmo display type|
|color|Color|Gizmo display color|
|gizmoSize|Vector3|Gizmo display size (for SPHERE, only X)|
|centerToCornerX|bool|Set X axis position as corner|
|centerToCornerY|bool|Set Y axis position as corner|
|centerToCornerZ|bool|Set Z axis position as corner|
|invertCornerX|bool|Set X axis position as invert corner|
|invertCornerY|bool|Set Y axis position as invert corner|
|invertCornerZ|bool|Set Z axis position as invert corner|

#### Enums

##### __GIZMO_TYPE__

|enums|description|
|:--|:--|
|CUBE|gizmo type cube|
|SPHERE|gizmo type sphere|
