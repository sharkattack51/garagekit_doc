# CommonUtil

ユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class CommonUtil
```

#### Static Methods

実行プラットフォームごとの外部リソースディレクトリを作成、取得する(WinMac:実行ファイルと同階層,　iOS:Application.persistentDataPath以下, Android:デバイスルート)
```csharp
public static string GetPlatformResourceRootDirectory(string appRootDir = "")
```

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
