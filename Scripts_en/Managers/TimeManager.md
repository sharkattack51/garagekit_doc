# TimeManager

Manage timer functions. Register and use [TimerEvent](~/Scripts_en/Utils/Event/TimerEvent.md). By default, MainTimer is registered.

```csharp
namespace GarageKit
public class TimeManager : ManagerBase
```

#### Inheritance

`TimeManager` -> [ManagerBase](~/Scripts_en/Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/timemanager_hierarchy.png" width="300px"/>
<br/>
<br/>
<img src="~/image/script_reference/timemanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|timerEvents|List<[TimerEvent](~/Scripts_en/Utils/Event/TimerEvent.md)>|タイマーイベントリスト|

#### Methods

Get reference to main timer
```csharp
public TimerEvent mainTimer { get; }
```

#### Example

```csharp
// Added timer completion event
AppMain.Instance.timeManager.mainTimer.OnCompleteTimer += (sender) => { Debug.Log("on complete timer"); };

// Start time count 10 seconds
AppMain.Instance.timeManager.mainTimer.StartTimer(10);
```
