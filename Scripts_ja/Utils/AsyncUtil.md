# AsyncUtil

Async 関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class AsyncUtil
```

#### Static Methods

Texture2D 非同期読み込み
```csharp
public static async UniTask<Texture2D> LoadTextureAsync(string path, CancellationToken ct = default)
```

Texture2D 複数同時の非同期読み込み
```csharp
public static async UniTask<Texture2D[]> LoadTextureAllAsync(string[] paths, CancellationToken ct = default)
```
