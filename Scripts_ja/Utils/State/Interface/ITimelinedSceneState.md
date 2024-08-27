# IStITimelinedSceneStateate

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) でタイムラインを利用した State 遷移を行うためのインターフェース

```csharp
namespace GarageKit
public interface ITimelinedSceneState
```

#### Methods

タイムラインを一時停止する処理の実装
```csharp
void Pause()
```

タイムラインを再開する処理の実装
```csharp
void Resume()
```

タイムラインが完了した際の処理の実装
```csharp
void OnStateTimer(GameObject sender)
```
