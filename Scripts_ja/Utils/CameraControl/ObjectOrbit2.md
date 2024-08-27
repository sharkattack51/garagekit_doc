# ObjectOrbit2

ドラッグ操作によりオブジェクトをターゲット中心にオービット回転させます。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
public class ObjectOrbit2
```

#### Inheritance

`ObjectOrbit2` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/objectorbit2_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|renderCam|Camera|Hit 判定用カメラ|
|sensitivity|float|操作感度|
|smoothTime|float|回転スムーズ量|
|invertRot|bool|回転方向反転設定|
|collidRadiusFromBounds|bool|判定用コライダーサイズをバウンディングから自動設定|
|collidRadius|float|判定用コライダー半径|

#### Methods

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
