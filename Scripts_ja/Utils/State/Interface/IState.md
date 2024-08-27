# IState

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で State 遷移を行うためのインターフェース

```csharp
namespace GarageKit
public interface IState
```

#### Methods

State 遷移後に State 内で最初に実行される処理の実装
```csharp
void StateStart(object context)
```

State 遷移後に State 内で毎フレーム実行される処理の実装
```csharp
void StateUpdate()
```

State 遷移時に State 内で最後に実行される処理の実装
```csharp
void StateExit()
```
