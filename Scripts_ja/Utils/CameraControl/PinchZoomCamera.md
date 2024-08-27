# PinchZoomCamera

マルチタッチのピンチ操作でのカメラズームを行います。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class PinchZoomCamera
```

#### Inheritance

`PinchZoomCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/pinchzoomcamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|zoomType|[PINCH_ZOOM_TYPE](#pinch_zoom_type)|ズーム処理タイプ|
|zoomBias|float|ズーム量|
|zoomSmoothTime|float|ズームスムーズ量|
|invertZoom|bool|ズーム方向反転設定|
|limitMinMaxForRelativePosZ|[LimitValue](#limitvalue)|Z 位置の相対値制限|
|limitMinMaxForFOV|[LimitValue](#limitvalue)|FOV 値制限|
|limitMinMaxForOrthoSize|[LimitValue](#limitvalue)|オルソカメラのサイズ値制限|
|disableComponents|MonoBehaviour[]|組み合わせ操作で OFF にするコンポーネント|
|zoomToPinchCenterFor2D|bool|2D ズーム時の中心をピンチ座標センターにする|
|ratioForWheel|float|マウスホイールでのズーム量|

#### Enums

##### __PINCH_ZOOM_TYPE__

|enums|description|
|:--|:--|
|POSITION_Z|Z 位置でのズーム|
|FOV|FOV 値でのズーム|
|ORTHOSIZE|オルソカメラのサイズ値でのズーム|

#### Methods

現在のズーム値
```csharp
public float currentZoom { get; }
```

入力ロックの確認
```csharp
public bool IsInputLock { get; }
```

入力のロック
```csharp
public void LockInput(object sender)
```

入力のロック解除
```csharp
public void UnlockInput(object sender)
```

指定量でズームさせる
```csharp
public void PushZoom(float zoomDelta)
```

目標値でズームさせる
```csharp
public void SetToPinchZoom(float zoom, float time = 1.0f)
```

ズームをリセット
```csharp
public void ResetPinchZoom()
```

#### Example

- /Scenes/Examples/CameraControllExample.unity

---

# LimitValue

最小最大制限値の構造体

```csharp
namespace GarageKit
[Serializable]
public class LimitValue
```

#### Properties

|member|type|description|
|:--|:--|:--|
|min|float|最小値|
|max|float|最大値|
