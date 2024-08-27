# CaptureUtil

Provides capture related utility functions.

```csharp
namespace GarageKit
public class CaptureUtil
```

#### Static Methods

Specify the range and save the screen capture
```csharp
public static IEnumerator CaptureRect(string fileName, bool withTimestamp)
public static IEnumerator CaptureRect(string dirPath, string fileName, Rect range, bool withTimestamp)
```
