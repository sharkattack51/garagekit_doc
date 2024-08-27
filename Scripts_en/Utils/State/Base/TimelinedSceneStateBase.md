# TimelinedSceneStateBase

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Base class for performing State transition using timeline.

```csharp
namespace GarageKit
public class TimelinedSceneStateBase : AsyncStateBase, ITimelinedSceneState
```

#### Inheritance

`TimelinedSceneStateBase` -> [AsyncStateBase](~/Scripts_en/Utils/State/Base/AsyncStateBase.md), [ITimelinedSceneState](~/Scripts_en/Utils/State/Interface/ITimelinedSceneState.md) -> [StateBase](~/Scripts_en/Utils/State/Base/StateBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/timelinedscenestatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|durationSec|int|Timeline length (seconds)|

#### Methods

Current timeline time
```csharp
public float CurrentActionTime { get; }
```

Check timeline playback
```csharp
public bool IsPlay { get; }
```

Check timeline it is paused
```csharp
public bool IsPaused { get; }
```

The first process executed within a State after a State transition
```csharp
public virtual void StateStart(object context)
```

Processing executed every frame within State after State transition
```csharp
public virtual void StateUpdate()
```

The last process executed within a State during a State transition
```csharp
public virtual void StateExit()
```

Process when timeline completes
```csharp
public virtual void OnStateTimer(GameObject sender)
```

Start timeline
```csharp
public void StartTimeline()
```

Pause timeline
```csharp
public virtual void Pause()
```

Resume timeline
```csharp
public virtual void Resume()
```
