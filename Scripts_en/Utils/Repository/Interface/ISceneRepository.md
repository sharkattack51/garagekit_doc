# ISceneRepository

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Repository object interface that provides inter-scene parameter access when using multiple scenes.

```csharp
namespace GarageKit
public interface ISceneRepository
```

#### Methods

Get value by string of variable name
```csharp
T FindByVarName<T>(string varName)
```
