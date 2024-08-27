# VRSceneStateBase

[SceneStateManager](~/Scripts_ja/Managers/SceneStateManager.md) でVR コンテンツ用の State 遷移を行うためのインターフェース

```csharp
namespace GarageKit
public interface VRSceneStateBase
```

#### Methods

現在のステートをリセットする処理の実装
```csharp
void ResetCurrentState()
```

表示オブジェクト設定処理の実装
```csharp
void SetStagingObjects();
```
