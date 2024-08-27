# ISceneRepository

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) で複数シーンを利用した場合のシーン間パラメータアクセスを提供するリポジトリオブジェクトのインターフェース

```csharp
namespace GarageKit
public interface ISceneRepository
```

#### Methods

変数名の文字列で値の取得
```csharp
T FindByVarName<T>(string varName)
```
