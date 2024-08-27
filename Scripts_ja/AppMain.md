# AppMain

シングルトンインスタンスで、各マネージャーへの参照経路を受け持ちます。

```csharp
namespace GarageKit
public class AppMain : MonoBehaviour
```

#### Inheritance

`AppMain` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/appmain_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|asDontDestroyOnLoad|bool|複数シーンで利用する場合に、シーン移動時に破棄されずにシーン間で共有される|

#### Static Methods

シングルトンインスタンスの取得
```csharp
public static AppMain Instance { get; }
```

#### Example

```csharp
// 各マネージャーへのルーティング
AppMain.Instance.sceneStateManager.ChangeState("PLAY");
AppMain.Instance.soundManager.Play("SE", "CLICK");
```
