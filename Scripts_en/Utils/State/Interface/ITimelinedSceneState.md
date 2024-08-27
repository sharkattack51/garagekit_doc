# IStITimelinedSceneStateate

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Interface for performing State transition using timeline.

```csharp
namespace GarageKit
public interface ITimelinedSceneState
```

#### Methods

Implementation of processing to pause the timeline
```csharp
void Pause()
```

Implementation of processing to rresume the timeline
```csharp
void Resume()
```

Implementation of processing when the timeline is completed
```csharp
void OnStateTimer(GameObject sender)
```
