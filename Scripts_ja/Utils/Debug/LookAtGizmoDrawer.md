# LookAtGizmoDrawer

SceneView に指定ターゲットまでのラインギズモを表示します。

<img src="~/image/script_reference/lookatgizmodrawer_sceneview.png" width="500px"/>
</br>
</br>

```csharp
namespace GarageKit
public class LookAtGizmoDrawer : MonoBehaviour
```

#### Inheritance

`LookAtGizmoDrawer` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/lookatgizmodrawer_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|color|Color|ギズモ表示カラー|
|target|GameObject|ライン終点のターゲット|
|worldUp|Vector3|上方向ベクトル|
