# FlyThroughCamera

ドラッグによるカメラのフライスルー操作を行います。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class FlyThroughCamera
```

#### Inheritance

`FlyThroughCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/flythroughcamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|groundCollider|Collider|地面判定用のコライダー|
|limitAreaCollider|Collider|移動制限用のコライダー|
|useLimitArea|bool|移動制限設定|
|moveBias|float|移動量|
|moveSmoothTime|float|移動スムーズ量|
|dragInvertX|bool|横ドラッグ方向反転設定|
|dragInvertY|bool|縦ドラッグ方向反転設定|
|rotateBias|float|方向回転量|
|rotateSmoothTime|float|方向回転スムーズ量|
|rotateInvert|bool|方向回転反転設定|
|combinationOrbitCamera|[OrbitCamera](~/Scripts_ja/Utils/CameraControl/OrbitCamera.md)|組み合わせ操作の対象コンポーネント|

#### Enums

##### __FLYTHROUGH_CONTROLL_TYPE__

|enums|description|
|:--|:--|
|DRAG|ドラッグで移動|
|DRAG_HOLD|ドラッグ後ホールドで移動|

##### __FLYTHROUGH_MOVE_TYPE__

|enums|description|
|:--|:--|
|XZ|XZ 平面操作|
|XY|XY 平面操作|

#### Methods

階層ルートの取得
```csharp
public GameObject FlyThroughRoot { get; }
```

位置シフト用ルートの取得
```csharp
public Transform ShiftTransform { get; }
```

現在の位置情報取得
```csharp
public Vector3 currentPos { get; }
```

現在の回転情報取得
```csharp
public Quaternion currentRot { get; }
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

目標位置にカメラをフライスルー移動させる
```csharp
public void MoveToFlyThrough(Vector3 targetPosition, float time = 1.0f)
```

指定量でカメラを即時移動させる
```csharp
public void TranslateToFlyThrough(Vector3 move)
```

目標方向にカメラをフライスルー回転させる
```csharp
public void RotateToFlyThrough(float targetAngle, float time = 1.0f)
```

指定量でカメラをフライスルー移動させる
```csharp
public void PushMove(Vector3 move)
```

指定量でカメラをフライスルー回転させる
```csharp
public void PushRotate(float rotate)
```

カメラの位置と回転をリセット
```csharp
public void ResetFlyThrough()
```

#### Example

- /Scenes/Examples/CameraControllExample.unity
