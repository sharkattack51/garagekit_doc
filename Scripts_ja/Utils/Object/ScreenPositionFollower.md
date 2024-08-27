# ScreenPositionFollower

ターゲットオブジェクトのスクリーン位置に同期させます。[GizmoDrawer](~/Scripts_ja/Utils/Debug/GizmoDrawer.md) と一緒に利用すると便利です。

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
|targetObject|GameObject|ターゲットの参照|
|rayCamera|Camera|スクリーンカメラの参照|
|screenWidth|int|スクリーン幅|
|screenHeight|int|スクリーン高さ|
|setAsScreenSize|bool|現在のスクリーンサイズを反映|
|uiScale|float|位置スケール|
