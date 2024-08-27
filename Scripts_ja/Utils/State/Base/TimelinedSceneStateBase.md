# TimelinedSceneStateBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) でタイムラインを利用した State 遷移を行うためのベースクラス

```csharp
namespace GarageKit
public class TimelinedSceneStateBase : AsyncStateBase, ITimelinedSceneState
```

#### Inheritance

`TimelinedSceneStateBase` -> [AsyncStateBase](~/Scripts_ja/Utils/State/Base/AsyncStateBase.md), [ITimelinedSceneState](~/Scripts_ja/Utils/State/Interface/ITimelinedSceneState.md) -> [StateBase](~/Scripts_ja/Utils/State/Base/StateBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/timelinedscenestatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|durationSec|int|タイムラインの尺（秒）|

#### Methods

現在のタイムライン時間
```csharp
public float CurrentActionTime { get; }
```

タイムラインの再生確認
```csharp
public bool IsPlay { get; }
```

タイムラインの一時停止確認
```csharp
public bool IsPaused { get; }
```

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

タイムラインが完了した際の処理
```csharp
public virtual void OnStateTimer(GameObject sender)
```

タイムラインを開始
```csharp
public void StartTimeline()
```

タイムラインを一時停止する処理
```csharp
public virtual void Pause()
```

タイムラインを再開する処理
```csharp
public virtual void Resume()
```
