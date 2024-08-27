# CameraGizmoDrawer

カメラオブジェクト非選択時にも SceneView に視錐台ギズモを表示します。

<img src="~/image/script_reference/cameragizmodrawer_sceneview.png" width="500px"/>
</br>
</br>

```csharp
namespace GarageKit
[ExecuteInEditMode]
[RequireComponent(typeof(Camera))]
public class CameraGizmoDrawer : MonoBehaviour
```

#### Inheritance

`CameraGizmoDrawer` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/cameragizmodrawer_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|gizmosColor|Color|ギズモ表示カラー|
