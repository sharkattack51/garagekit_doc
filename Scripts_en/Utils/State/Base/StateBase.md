# StateBase

Base class for performing State transitions in [SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md).

```csharp
namespace GarageKit
public class StateBase : MonoBehaviour, IState
```

#### Inheritance

`StateBase` -> `MonoBehaviour`, [IState](~/Scripts_en/Utils/State/Interface/IState.md)

#### Properties

|member|type|description|
|:--|:--|:--|
|updateEnable|bool|Can be used to enable/disable StateUpdate() processing|

#### Methods

Checking the validity of StateUpdate() processing
```csharp
public bool IsUpdateEnable { get; }
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
