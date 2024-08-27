# CameraShifter

カメラシフトを行います。projectionMatrix が内部で上書きされるのでカメラ FOV 設定は無効になります。

```csharp
namespace GarageKit
public class CameraShifter
```

#### Inheritance

`CameraShifter` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/camerashifter_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|shiftX|float|横方向シフトの割合|
|shiftY|float|縦方向シフトの割合|
|calcAlways|bool|Update 更新設定|

#### Methods

初期状態へリセット
```csharp
public void ResetProjMat()
```