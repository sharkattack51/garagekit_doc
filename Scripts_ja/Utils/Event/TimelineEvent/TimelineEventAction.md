# TimelineEventAction

[TimelinedSceneStateBase](~/Scripts_ja/Utils/State/Base/TimelinedSceneStateBase.md) で利用するタイムラインイベントの登録アクションデータ構造体

```csharp
namespace GarageKit
public class TimelineEventAction
```

#### Inheritance

`TimelineEventAction`

#### Properties

|member|type|description|
|:--|:--|:--|
|time|float|経過時間|

#### Methods

経過時間での登録アクション
```csharp
public Action action;
```

アクション完了確認
```csharp
public bool IsDone { get； }
```
