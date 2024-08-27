# AsyncStateBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) でフェード付き State 遷移を行うためのベースクラス

```csharp
namespace GarageKit
public class AsyncStateBase : StateBase, IAsyncState
```

#### Inheritance

`AsyncStateBase` -> [StateBase](~/Scripts_ja/Utils/State/Base/StateBase.md), [IAsyncState](~/Scripts_ja/Utils/State/Interface/IAsyncState.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/asyncstatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|fadeTime|float|フェード時間|
|fadeColor|Color|フェードカラー|

#### Methods

State 遷移後に State 内で最初に実行される処理
```csharp
public virtual void StateStart(object context)
```

State 遷移後に State 内で毎フレーム実行される処理
```csharp
public virtual void StateUpdate()
```

State 遷移時に State 内で最後に実行される処理
```csharp
public virtual void StateExit()
```

フェード完了後に実行される処理
```csharp
public virtual void StateExitAsync()
```
