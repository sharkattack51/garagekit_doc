# SceneRepositoryBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で複数シーンを利用した場合のシーン間パラメータアクセスを提供するリポジトリオブジェクト。遷移先シーンをロード後、遷移先シーンに配置済みの SceneRepositoryBase を経由してインスペクタ設定済みの参照を取得可能です。

```csharp
namespace GarageKit
public class SceneRepositoryBase : MonoBehaviour, ISceneRepository
```

#### Inheritance

`SceneRepositoryBase` -> `MonoBehaviour`, `ISceneRepository`

#### Methods

変数名の文字列で値の取得
```csharp
public T FindByVarName<T>(string varName)
```

#### Example

```csharp
// sample repository class
public class MultipleSceneRepository : SceneRepositoryBase
{
    public Text messageText;
    public GameObject testCube;
}
```

[MultipleSceneStateBase](~/Scripts_ja/Utils/State/Base/MultipleSceneStateBase.md)

```csharp
// 遷移先シーンをロード後、遷移先シーンに配置済みの SceneRepositoryBase を経由してインスペクタ設定済みの参照を取得可能
string text = (this.SceneRepository as MultipleSceneRepository).messageText.text;
GameObject cube = (this.SceneRepository as MultipleSceneRepository).testCube;
```