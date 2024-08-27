# MultipleSceneStateBase

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Base class for performing State transition using multiple scenes.

```csharp
namespace GarageKit
public class MultipleSceneStateBase : StateBase, IAsyncState
```

#### Inheritance

`MultipleSceneStateBase` -> [StateBase](~/Scripts_en/Utils/State/Base/StateBase.md), [IMultipleSceneState](~/Scripts_en/Utils/State/Interface/IMultipleSceneState.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/multiplescenestatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|loadSceneName|string|Scene name to load correspondingly|
|asAsyncLoad|bool|Scene asynchronous loading settings|
|asAdditiveLoad|bool|Additional scene loading settings|

#### Methods

Get [SceneRepository](~/Scripts_en/Utils/Repository/Base/SceneRepositoryBase.md)
```csharp
public SceneRepositoryBase SceneRepository { get; }
```

The first process executed within a State after a State transition
```csharp
public virtual void StateStart(object context)
```

Processing executed after scene loading is complete
```csharp
public virtual void SceneLoaded()
```

Processing executed every frame within State after State transition
```csharp
public virtual void StateUpdate()
```

The last process executed within a State during a State transition
```csharp
public virtual void StateExit()
```

Processing executed after scene destruction
```csharp
public virtual void SceneUnloaded()
```
