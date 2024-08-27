# StateBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で State 遷移を行うためのベースクラス

```csharp
namespace GarageKit
public class StateBase : MonoBehaviour, IState
```

#### Inheritance

`StateBase` -> `MonoBehaviour`, [IState](~/Scripts_ja/Utils/State/Interface/IState.md)

#### Properties

|member|type|description|
|:--|:--|:--|
|updateEnable|bool|StateUpdate() 処理の有効 / 無効の設定に利用可能|

#### Methods

StateUpdate() 処理の有効確認
```csharp
public bool IsUpdateEnable { get; }
```

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
