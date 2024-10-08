# CommonUtil

ユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class CommonUtil
```

#### Static Methods

ファイルブラウザで指定フォルダを開く
```csharp
public static void OpenFolder(string path)
```

対象ディレクトリのコピー
```csharp
public static void CopyDirectory(string src, string dest, bool overwriteAsLatest = true)
```

非同期で対象ディレクトリのコピー
```csharp
public static async UniTask CopyDirectoryAsync(string src, string dest, bool overwriteAsLatest = true, CancellationToken ct = default)
```
