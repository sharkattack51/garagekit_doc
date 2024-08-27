# AndroidUtil

Provides utility functions for Android.

```csharp
namespace GarageKit
public class AndroidUtil
```

#### Static Methods

Get path to internal data area
```csharp
public static string FileDir()
```

Get path to internal cache area
```csharp
public static string CacheDir()
```

Get path to external data area
```csharp
public static string ExternalFilesDir()
```

Get path to external cache area
```csharp
public static string ExternalCacheDir()
```

Get path to external strage
```csharp
public static string ExternalStorageDir()
```

Get path to public area in external strage
```csharp
public static string ExternalStoragePublicDir()
```

Get path to download directory
```csharp
public static string DownloadDir()
```

Open specified activity
```csharp
public static void OpenActivity(string packageName, string className, bool asNewTask)
```

Sending broadcast messages to the system
```csharp
public static void SendBroadcast(string action)
```

Get API level
```csharp
public static int GetApiLevel()
```

Requesting file access permissions on Android 11 and above
```csharp
public static void RequestAllFilesAccessPermission()
```
