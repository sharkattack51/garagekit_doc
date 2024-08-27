# TimelineEventAction

Registration action data structure for timeline events used in [TimelinedSceneStateBase](~/Scripts_en/Utils/State/Base/TimelinedSceneStateBase.md).

```csharp
namespace GarageKit
public class TimelineEventAction
```

#### Inheritance

`TimelineEventAction`

#### Properties

|member|type|description|
|:--|:--|:--|
|time|float|Elapsed time|

#### Methods

Registration action with elapsed time
```csharp
public Action action;
```

Check action completion
```csharp
public bool IsDone { get； }
```
