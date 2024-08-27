# MultipleSceneAsyncStateBase

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Base class for performing state transition with fade using multiple scenes.

```csharp
namespace GarageKit
public class MultipleSceneAsyncStateBase : MultipleSceneStateBase, IAsyncState
```

#### Inheritance

`MultipleSceneAsyncStateBase` -> [MultipleSceneStateBase](~/Scripts_en/Utils/State/Base/MultipleSceneStateBase.md), [IAsyncState](~/Scripts_en/Utils/State/Interface/IAsyncState.md) -> [StateBase](~/Scripts_en/Utils/State/Base/StateBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/multiplesceneasyncstatebase_inspector.png" width="500px"/>

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

Processing executed after the fade is completed
```csharp
public virtual void StateExitAsync()
```
