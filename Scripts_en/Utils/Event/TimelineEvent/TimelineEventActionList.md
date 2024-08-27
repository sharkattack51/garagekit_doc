# TimelineEventActionList

Registration action data list structure for timeline events used in [TimelinedSceneStateBase](~/Scripts_en/Utils/State/Base/TimelinedSceneStateBase.md)

```csharp
namespace GarageKit
public class TimelineEventActionList
```

#### Inheritance

`TimelineEventActionList`

#### Methods

Execute registration action with elapsed time
```csharp
public void Update(float time)
```

New action registration
```csharp
public void Add(float time, Action action)
```

Clear registered action list
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
