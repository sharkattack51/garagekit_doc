# ARCameraSync

AR カメラオブジェクトとパラメータを同期させます。

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit.ARFoundationExtention
[RequireComponent(typeof(Camera))]
public class ARCameraSync : MonoBehaviour
```

#### Inheritance

`ARCameraSync` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arcamerasync_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|arCameraManager|ARCameraManager|ARCameraManager の参照|
|syncFov|bool|カメラ FOV の同期設定|
|syncPosition|bool|Position の同期設定|
|syncRotation|bool|Rotation の同期設定|
|asLocal|bool|ローカル座標系での同期|
