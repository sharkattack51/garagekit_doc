# VRSceneStateBase

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Base class for performing state transitions for VR content。

```csharp
namespace GarageKit
public class VRSceneStateBase : TimelinedSceneStateBase, ISequentialState, IVRSceneState
```

#### Inheritance

`VRSceneStateBase` -> [TimelinedSceneStateBase](~/Scripts_en/Utils/State/Base/TimelinedSceneStateBase.md), [ISequentialState](~/Scripts_en/Utils/State/Interface/ISequentialState.md), [IVRSceneState](~/Scripts_en/Utils/State/Interface/IVRSceneState.md) -> [AsyncStateBase](~/Scripts_en/Utils/State/Base/AsyncStateBase.md) -> [StateBase](~/Scripts_en/Utils/State/Base/StateBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/vrscenestatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|viewReferenceObj|GameObject|Reference of viewpoint position object|
|viewGuideTarget|GameObject|Reference to gaze guide object|
|enables|[StageManagedObject](~/Scripts_en/Utils/Object/StageManagedObject.md)[]|Display management object list|

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

Transition processing to the next State
```csharp
public virtual void ToNextState()
```

Transition process to previous State
```csharp
public virtual void ToPrevState()
```

Processing to reset the current state
```csharp
public virtual void ResetCurrentState()
```

Display object setting processing
```csharp
public void SetStagingObjects()
```
