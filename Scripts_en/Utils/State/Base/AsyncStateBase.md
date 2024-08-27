# AsyncStateBase

Base class for performing State transition with fade in [SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md)

```csharp
namespace GarageKit
public class AsyncStateBase : StateBase, IAsyncState
```

#### Inheritance

`AsyncStateBase` -> [StateBase](~/Scripts_en/Utils/State/Base/StateBase.md), [IAsyncState](~/Scripts_en/Utils/State/Interface/IAsyncState.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/asyncstatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|fadeTime|float|Fade time|
|fadeColor|Color|Fade color|

#### Methods

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

Processing executed after the fade is completed
```csharp
public virtual void StateExitAsync()
```
