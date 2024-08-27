# SceneStateManager

Manage state transition functionality. Place and manage state objects that inherit [StateBase](../Utils/State/Base/StateBase.md) under the SceneStateManager hierarchy.  

```csharp
namespace GarageKit
public class SceneStateManager : ManagerBase
```

#### Inheritance

`SceneStateManager` -> [ManagerBase](../Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/scenestatemanager_hierarchy.png" width="300px"/>
<br/>
<br/>
<img src="~/image/script_reference/scenestatemanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|sceneStateTable|List<[SceneStateData](#scenestatedata)>|State transition information table|

#### Methods

Current state information
```csharp
public SceneStateData CurrentState { get; }
```

Previous state name
```csharp
public string FromStateName { get; }
```

State transition processing flag
```csharp
public bool StateChanging { get; }
```

State transition fade processing flag
```csharp
public bool AsyncChangeFading { get; }
```

State initialization completion flag
```csharp
public bool StateInitted { get; }
```

Get state object from scene
```csharp
public T FindStateObjectOfType<T>() where T : StateBase
public StateBase FindStateObjectByName(string stateName)
```

Transition to initial state. called `WaitForEndOfFrame()` from `Start()` in AppMain.
```csharp
public void InitState()
```

Transition to specified state
```csharp
public void ChangeState(string stateName, object context = null)
```

Transition with fade to specified state
```csharp
public void ChangeAsyncState(string stateName, object context = null)
```

#### Example

```csharp
// Transition to specified state
AppMain.Instance.sceneStateManager.ChangeState("PLAY");

// Transition with fade by passing parameters to specified state
AppMain.Instance.sceneStateManager.ChangeAsyncState("PLAY", "param");
```

---

# SceneStateData

State transition information structure

```csharp
namespace GarageKit
[Serializable]
public class SceneStateData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|stateName|string|State name|
|stateObj|[StateBase](../Utils/State/Base/StateBase.md)|Reference to state object|
|asInitial|bool|Initial state flag|
