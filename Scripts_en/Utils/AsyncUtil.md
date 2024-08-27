# AsyncUtil

Provides Async-related utility functions.

```csharp
namespace GarageKit
public class AsyncUtil
```

#### Static Methods

Texture2D asynchronous loading
```csharp
public static async UniTask<Texture2D> LoadTextureAsync(string path, CancellationToken ct = default)
```

Texture2D multiple simultaneous asynchronous loading
```csharp
public static async UniTask<Texture2D[]> LoadTextureAllAsync(string[] paths, CancellationToken ct = default)
```
