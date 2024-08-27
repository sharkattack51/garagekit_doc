# DebugManager

Manage functions for debugging. It is useful to have all debugging functionality managed by the isDebug flag.

```csharp
namespace GarageKit
[RequireComponent(typeof(VisibleMouseCursor))]
public class DebugManager : ManagerBase
```

#### Inheritance

`DebugManager` -> [ManagerBase](../Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/debugmanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|isDebug|bool|Debug state management flag|
|useIngameDebugConsole|bool|use package [IngameDebugConsole](https://openupm.com/packages/com.yasirkula.ingamedebugconsole/)|
|useGraphy|bool|use package [Graphy](https://openupm.com/packages/com.tayx.graphy/)|

#### Example

```csharp
// Check debug status
if(AppMain.Instance.debugManager.isDebug)
    Debug.Log("debug is true");
```
