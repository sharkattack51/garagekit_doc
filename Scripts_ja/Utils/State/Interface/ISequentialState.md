# ISequentialState

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で連続した State 遷移を行うためのインターフェース

```csharp
namespace GarageKit
public interface ISequentialState
```

#### Methods

次の State への遷移処理の実装
```csharp
void ToNextState()
```

前の State への遷移処理の実装
```csharp
void ToNextState()
```