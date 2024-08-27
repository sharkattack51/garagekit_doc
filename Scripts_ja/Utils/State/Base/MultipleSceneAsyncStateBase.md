# MultipleSceneAsyncStateBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で複数シーンを利用したフェード付き State 遷移を行うためのベースクラス

```csharp
namespace GarageKit
public class MultipleSceneAsyncStateBase : MultipleSceneStateBase, IAsyncState
```

#### Inheritance

`MultipleSceneAsyncStateBase` -> [MultipleSceneStateBase](~/Scripts_ja/Utils/State/Base/MultipleSceneStateBase.md), [IAsyncState](~/Scripts_ja/Utils/State/Interface/IAsyncState.md) -> [StateBase](~/Scripts_ja/Utils/State/Base/StateBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/multiplesceneasyncstatebase_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|loadSceneName|string|対応して読み込むシーン名|
|asAsyncLoad|bool|シーンの非同期読み込み設定|
|asAdditiveLoad|bool|シーンの追加読み込み設定|

#### Methods

[SceneRepository](~/Scripts_ja/Utils/Repository/Base/SceneRepositoryBase.md) の取得
```csharp
public SceneRepositoryBase SceneRepository { get; }
```

State 遷移後に State 内で最初に実行される処理
```csharp
public virtual void StateStart(object context)
```

シーン読み込み完了後に実行される処理
```csharp
public virtual void SceneLoaded()
```

State 遷移後に State 内で毎フレーム実行される処理
```csharp
public virtual void StateUpdate()
```

State 遷移時に State 内で最後に実行される処理
```csharp
public virtual void StateExit()
```

フェード完了後に実行される処理の実装
```csharp
public virtual void StateExitAsync()
```
