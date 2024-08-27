# IState

Interface for performing State transition in [SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md).

```csharp
namespace GarageKit
public interface IState
```

#### Methods

Implementation of the first process executed within a State after a State transition
```csharp
void StateStart(object context)
```

Implementation of processing executed every frame within State after State transition
```csharp
void StateUpdate()
```

Implementation of the last process executed within a State during a State transition
```csharp
void StateExit()
```
