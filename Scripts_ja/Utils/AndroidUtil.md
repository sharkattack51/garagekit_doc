# AndroidUtil

Android 用のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class AndroidUtil
```

#### Static Methods

デバイスの内部データ領域へのパスを取得
```csharp
public static string FileDir()
```

デバイスの内部キャッシュ領域へのパスを取得
```csharp
public static string CacheDir()
```

デバイスの外部データ領域へのパスを取得
```csharp
public static string ExternalFilesDir()
```

デバイスの外部キャッシュ領域へのパスを取得
```csharp
public static string ExternalCacheDir()
```

デバイスの外部ストレージ領域へのパスを取得
```csharp
public static string ExternalStorageDir()
```

デバイスの外部ストレージ共有領域へのパスを取得
```csharp
public static string ExternalStoragePublicDir()
```

デバイスのダウンロードフォルダへのパスを取得
```csharp
public static string DownloadDir()
```

指定したアクティビティを開く
```csharp
public static void OpenActivity(string packageName, string className, bool asNewTask)
```

システムへブロードキャストメッセージの送信
```csharp
public static void SendBroadcast(string action)
```

APIレベルの取得
```csharp
public static int GetApiLevel()
```

Android 11 以上でファイルアクセスパーミッションのリクエスト
```csharp
public static void RequestAllFilesAccessPermission()
```
