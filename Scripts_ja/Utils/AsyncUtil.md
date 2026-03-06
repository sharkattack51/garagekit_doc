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

Texture2D オプションを指定して非同期読み込み
```csharp
public static async UniTask<Texture2D> LoadTextureWithOptionAsync(string path, TextureFormat texFormat, bool mipChain, TextureWrapMode wrapModeU, TextureWrapMode wrapModeV, FilterMode filterMode, CancellationToken ct = default)
```

非同期ダウンロード
```csharp
public static async UniTask<string> DownloadAsync(string url, CancellationToken ct = default)
```

非同期ダウンロード後にファイル保存
```csharp
public static async UniTask DownloadFileAsync(string url, string dstFile, CancellationToken ct = default)
```

複数対象を非同期ダウンロード後にファイル保存
```csharp
public static async UniTask DownloadFileAllAsync(string[] urls, string[] dstFiles, CancellationToken ct = default)
```
