# PanoramaOrbit

パノラマ用オブジェクトをオービット回転操作します。カメラを回転させる場合は [Panorama360Camera](~/Scripts_ja/Utils/CameraControl/Panorama360Camera.md) も利用できます。

```csharp
namespace GarageKit
public class PanoramaOrbit : MonoBehaviour, ILocalize
```

#### Inheritance

`PanoramaOrbit` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/panoramaorbit_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|mode|[OPERATION_MODE](#operation_mode)|回転操作モード|
|rotationSpeed|float|回転速度|
|invertY|bool|Y 軸回転の反転設定|
|invertX|bool|X 軸回転の反転設定|

#### Enums

##### __OPERATION_MODE__

|enums|description|
|:--|:--|
|ROTATE_Y|Y 軸回転操作|
|ROTATE_XY|X 軸 Y 軸回転操作|

#### Methods

回転のリセット
```csharp
public void RotationReset()
```

回転値のセット
```csharp
public void SetRotate(float h, float v, float speed)
```
