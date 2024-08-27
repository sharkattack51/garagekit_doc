# Panorama360Camera

パノラマ 360° のカメラ操作を行います。

```csharp
namespace GarageKit
public class Panorama360Camera
```

#### Inheritance

`Panorama360Camera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/panorama360camera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|mode|[OPERATION_MODE](#operation_mode)|操作モード|
|rotationSpeed|float|回転スピード|
|useLimit|bool|回転制限設定|
|limitRotL|float|左回転方向の制限角度|
|limitRotR|float|右回転方向の制限角度|
|invertRotH|bool|横回転方向の反転設定|
|invertRotV|bool|縦回転方向の反転設定|
|useSmooth|bool|回転スムーズ設定|
|smoothTime|float|回転スムーズ量|

#### Enums

##### __OPERATION_MODE__

|enums|description|
|:--|:--|
|GYRO|ジャイロ操作|
|DRAG_MOUSE|マウス操作|
|DRAG_TOUCH|タッチ操作|
|GAME_PAD|ゲームパッド操作|

#### Methods

ジャイロをリセット
```csharp
public void ResetGyro()
```

カメラの回転をリセット
```csharp
public void ResetRotation(bool force = false)
```

カメラの回転値を設定
```csharp
public void SetRotate(float h, float v, float speed)
```

#### Example

- /Scenes/Examples/CameraControllExample.unity
