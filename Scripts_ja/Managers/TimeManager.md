# TimeManager

タイマー機能を管理します。[TimerEvent](~/Scripts_ja/Utils/Event/TimerEvent.md) を登録して利用します。デフォルトでは MainTimer を登録しています。

```csharp
namespace GarageKit
public class TimeManager : ManagerBase
```

#### Inheritance

`TimeManager` -> [ManagerBase](~/Scripts_ja/Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/timemanager_hierarchy.png" width="300px"/>
<br/>
<br/>
<img src="~/image/script_reference/timemanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|timerEvents|List<[TimerEvent](~/Scripts_ja/Utils/Event/TimerEvent.md)>|タイマーイベントリスト|

#### Methods

メインタイマーへの参照取得
```csharp
public TimerEvent mainTimer { get; }
```

#### Example

```csharp
// タイマー完了イベントを追加
AppMain.Instance.timeManager.mainTimer.OnCompleteTimer += (sender) => { Debug.Log("on complete timer"); };

// タイムカウント10秒sを開始
AppMain.Instance.timeManager.mainTimer.StartTimer(10);
```
