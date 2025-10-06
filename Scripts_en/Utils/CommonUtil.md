# CommonUtil

Provides utility functions.

```csharp
namespace GarageKit
public class CommonUtil
```

#### Static Methods

Create and retrieve external resource directories for each execution platform (WinMac: same hierarchy as the executable, iOS: Application.persistentDataPath, Android: device root)
```csharp
public static string GetPlatformResourceRootDirectory(string appRootDir = "")
```

Open the specified folder in the file browser
```csharp
public static void OpenFolder(string path)
```

Copy target directory
```csharp
public static void CopyDirectory(string src, string dest, bool overwriteAsLatest = true)
```

Copy target directory asynchronously
```csharp
public static async UniTask CopyDirectoryAsync(string src, string dest, bool overwriteAsLatest = true, CancellationToken ct = default)
```
