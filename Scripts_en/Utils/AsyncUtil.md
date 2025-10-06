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

Asynchronous downlod
```csharp
public static async UniTask<string> DownloadAsync(string url, CancellationToken ct = default)
```

Save file after asynchronous download
```csharp
public static async UniTask DownloadFileAsync(string url, string dstFile, CancellationToken ct = default)
```

Save files after asynchronous download of multiple targets
```csharp
public static async UniTask DownloadFileAllAsync(string[] urls, string[] dstFiles, CancellationToken ct = default)
```
