# ScreenPositionFollower

Synchronize to the screen position of the target object. It is useful to use it together with [GizmoDrawer](~/Scripts_en/Utils/Debug/GizmoDrawer.md).

```csharp
namespace GarageKit
public class ScreenPositionFollower : MonoBehaviour
```

#### Inheritance

`ScreenPositionFollower` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/screenpositionfollower_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|targetObject|GameObject|Target reference|
|rayCamera|Camera|Screen camera reference|
|screenWidth|int|Screen width|
|screenHeight|int|Screen height|
|setAsScreenSize|bool|Reflects current screen size|
|uiScale|float|Scale|
