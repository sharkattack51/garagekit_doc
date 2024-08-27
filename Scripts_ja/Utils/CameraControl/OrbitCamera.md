# OrbitCamera

ドラッグ操作によりカメラをターゲット中心にオービット回転させます。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class OrbitCamera
```

#### Inheritance

`OrbitCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/orbitcamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|orbitInputType|[ORBIT_INPUT_TYPE](#orbit_input_type)|操作入力タイプ|
|target|GameObject|回転中心ターゲット|
|sensitivity|float|操作感度|
|smoothTime|float|回転スムーズ量|
|clampRotationX_Min|float|X 回転の制限 最小値|
|clampRotationX_Max|float|X 回転の制限 最大値|
|invertDragX|bool|横ドラッグ方向反転設定|
|invertDragY|bool|縦ドラッグ方向反転設定|
|ratioForMouse|float|マウス操作時の回転量|
|combinationFlyThroughCamera|[FlyThroughCamera](~/Scripts_ja/Utils/CameraControl/FlyThroughCamera.md)|組み合わせ操作の対象コンポーネント|

#### Enums

##### __ORBIT_INPUT_TYPE__

|enums|description|
|:--|:--|
|PRIMARY|プライマリ入力|
|SECONDARY|セカンダリ入力|

#### Methods

階層ルートの取得
```csharp
public GameObject OrbitRoot { get; }
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

回転をリセット
```csharp
public void ResetOrbit()
```

#### Example

- /Scenes/Examples/CameraControllExample.unity
