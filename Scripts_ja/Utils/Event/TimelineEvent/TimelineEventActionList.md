# TimelineEventActionList

[TimelinedSceneStateBase](~/Scripts_ja/Utils/State/Base/TimelinedSceneStateBase.md) で利用するタイムラインイベントの登録アクションデータリスト構造体

```csharp
namespace GarageKit
public class TimelineEventActionList
```

#### Inheritance

`TimelineEventActionList`

#### Methods

経過時間で登録アクションを実行
```csharp
public void Update(float time)
```

新規アクション登録
```csharp
public void Add(float time, Action action)
```

登録アクションリストをクリア
```csharp
public void Clear()
```

#### Example

- /Scenes/Examples/EventExample.unity
- /Scenes/Examples/TimelinedStateExample.unity

```csharp
// TimelinedSceneStateBase.cs

this.actionList = new TimelineEventActionList();
this.actionList.Add(0.0f, () => {
    sceneText.text = "start";
});
this.actionList.Add(5.0f, () => {
    sceneText.text = "5 sec elapsed";
});
this.actionList.Add(10.0f, () => {
    sceneText.text = "10 sec elapsed";
});
this.actionList.Add(20.0f, () => {
    sceneText.text = "20 sec elapsed";
});
this.StartTimeline();
```
