# GrabMove

マルチタッチのグラブ操作でオブジェクトを移動させます。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit
public class GrabMove
```

#### Inheritance

`GrabMove` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/grabmove_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|renderCamera|Camera|ヒット判定用のカメラ|
|grabTouchNum|int|マルチタッチ操作時の判定用タッチ本数|
|moveBias|float|移動量|
|smoothTime|float|移動スムーズ量|
|disableComponents|MonoBehaviour[]|組み合わせ操作で OFF にするコンポーネント|

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

初期位置にリセット
```csharp
public void ResetGrabMove()
```
