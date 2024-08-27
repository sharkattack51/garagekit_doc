# SceneStateManager

ステート遷移機能を管理します。[StateBase](~/Scripts_ja/Utils/State/Base/StateBase.md) を継承したステートオブジェクトを SceneStateManager 階層下に配置して管理します。

```csharp
namespace GarageKit
public class SceneStateManager : ManagerBase
```

#### Inheritance

`SceneStateManager` -> [ManagerBase](~/Scripts_ja/Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/scenestatemanager_hierarchy.png" width="300px"/>
<br/>
<br/>
<img src="~/image/script_reference/scenestatemanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|sceneStateTable|List<[SceneStateData](#scenestatedata)>|ステート遷移情報テーブル|

#### Methods

現在のステート情報
```csharp
public SceneStateData CurrentState { get; }
```

一つ前のステート名
```csharp
public string FromStateName { get; }
```

ステート遷移処理中フラグ
```csharp
public bool StateChanging { get; }
```

ステート遷移フェード処理中フラグ
```csharp
public bool AsyncChangeFading { get; }
```

ステート初期化完了フラグ
```csharp
public bool StateInitted { get; }
```

シーンからステートオブジェクトの取得
```csharp
public T FindStateObjectOfType<T>() where T : StateBase
public StateBase FindStateObjectByName(string stateName)
```

初期ステートへの遷移（AppMain の `Start()` から `WaitForEndOfFrame()` 後に呼ばれる）
```csharp
public void InitState()
```

指定ステートへの遷移
```csharp
public void ChangeState(string stateName, object context = null)
```

指定ステートへのフェード付き遷移
```csharp
public void ChangeAsyncState(string stateName, object context = null)
```

#### Example

```csharp
// 指定ステートへの遷移
AppMain.Instance.sceneStateManager.ChangeState("PLAY");

// 指定ステートへパラメータを渡してのフェード付き遷移　
AppMain.Instance.sceneStateManager.ChangeAsyncState("PLAY", "param");
```

---

# SceneStateData

ステート遷移情報の構造体

```csharp
namespace GarageKit
[Serializable]
public class SceneStateData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|stateName|string|ステート名|
|stateObj|[StateBase](~/Scripts_ja/Utils/State/Base/StateBase.md)|ステートオブジェクトの参照|
|asInitial|bool|初期ステートフラグ|
