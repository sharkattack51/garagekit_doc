# SceneRepositoryBase

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) is a repository object that provides inter-scene parameter access when using multiple scenes. After loading the destination scene, you can obtain the inspector-configured reference via the SceneRepositoryBase placed in the destination scene.

```csharp
namespace GarageKit
public class SceneRepositoryBase : MonoBehaviour, ISceneRepository
```

#### Inheritance

`SceneRepositoryBase` -> `MonoBehaviour`, `ISceneRepository`

#### Methods

Get value by string of variable name
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

[MultipleSceneStateBase](~/Scripts_en/Utils/State/Base/MultipleSceneStateBase.md)

```csharp
// After loading the destination scene, you can get the inspector-configured reference via the SceneRepositoryBase placed in the destination scene.
string text = (this.SceneRepository as MultipleSceneRepository).messageText.text;
GameObject cube = (this.SceneRepository as MultipleSceneRepository).testCube;
```