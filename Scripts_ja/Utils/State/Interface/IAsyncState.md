# IAsyncState

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) でフェード付き State 遷移を行うためのインターフェース

```csharp
namespace GarageKit
public interface IAsyncState
```

#### Methods

フェード完了後に実行される処理の実装
```csharp
void StateExitAsync()
```
