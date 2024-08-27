# VRSceneStateBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) でVR コンテンツ用の State 遷移を行うためのベースクラス

```csharp
namespace GarageKit
public class VRSceneStateBase : TimelinedSceneStateBase, ISequentialState, IVRSceneState
```

#### Inheritance

`VRSceneStateBase` -> [TimelinedSceneStateBase](~/Scripts_ja/Utils/State/Base/TimelinedSceneStateBase.md), [ISequentialState](~/Scripts_ja/Utils/State/Interface/ISequentialState.md), [IVRSceneState](~/Scripts_ja/Utils/State/Interface/IVRSceneState.md) -> [AsyncStateBase](~/Scripts_ja/Utils/State/Base/AsyncStateBase.md) -> [StateBase](~/Scripts_ja/Utils/State/Base/StateBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/vrscenestatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|viewReferenceObj|GameObject|視点位置オブジェクトの参照|
|viewGuideTarget|GameObject|視線先ガイドオブジェクトの参照|
|enables|[StageManagedObject](~/Scripts_ja/Utils/Object/StageManagedObject.md)[]|表示管理オブジェクトリスト|

#### Methods

State 遷移後に State 内で最初に実行される処理
```csharp
public virtual void StateStart(object context)
```

State 遷移後に State 内で毎フレーム実行される処理
```csharp
public virtual void StateUpdate()
```

State 遷移時に State 内で最後に実行される処理
```csharp
public virtual void StateExit()
```

次の State への遷移処理
```csharp
public virtual void ToNextState()
```

前の State への遷移処理
```csharp
public virtual void ToPrevState()
```

現在のステートをリセットする処理
```csharp
public virtual void ResetCurrentState()
```

表示オブジェクト設定処理
```csharp
public void SetStagingObjects()
```
