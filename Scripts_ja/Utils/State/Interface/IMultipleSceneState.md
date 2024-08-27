# IMultipleSceneState

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で複数シーンを利用した State 遷移を行うためのインターフェース

```csharp
namespace GarageKit
public interface IMultipleSceneState
```

#### Methods

シーン読み込み完了後に実行される処理の実装
```csharp
void SceneLoaded()
```
