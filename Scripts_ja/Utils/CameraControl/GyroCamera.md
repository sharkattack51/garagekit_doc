# GyroCamera

ジャイロでカメラ回転を操作します。

> [!IMPORTANT]
> GyroDroid パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
public class GyroCamera
```

#### Inheritance

`GyroCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/gyrocamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|northDirection|[NORTH_DIRECTION](#north_direction)|基準方向(北)の設定|

#### Enums

##### __NORTH_DIRECTION__

|enums|description|
|:--|:--|
|NONE|なし|
|COMPASS_NORTH|コンパス機能の北方向|
|GYRO_HEAD_DIRECTION|ジャイロの Z 方向|

#### Methods

準備完了の確認
```csharp
public bool IsReady { get; }
```

準備完了時コールバック
```csharp
public Action OnReady
```

現在の Z を基準方向(北)に設定
```csharp
public void CalibrateNorth()
```

カメラ FOV の変更
```csharp
public void SetFov(float fov)
```
