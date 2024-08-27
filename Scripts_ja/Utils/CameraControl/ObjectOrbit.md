# ObjectOrbit

ドラッグ操作によりオブジェクトをターゲット中心にオービット回転させます。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
public class ObjectOrbit
```

#### Inheritance

`ObjectOrbit` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/objectorbit_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|sensitivity|float|操作感度|
|speed|float|回転速度|
|smoothTime|float|回転スムーズ量|
|clampRotationX|bool|X 回転の制限|
|clampRotationX_Min|float|X 回転の制限 最小値|
|clampRotationX_Max|float|X 回転の制限 最大値|
|invertDragX|bool|横ドラッグ方向反転設定|
|invertDragY|bool|縦ドラッグ方向反転設定|

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

回転をリセット
```csharp
public void ResetOrbit()
```