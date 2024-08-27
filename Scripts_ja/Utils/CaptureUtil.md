# CaptureUtil

キャプチャ関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class CaptureUtil
```

#### Static Methods

範囲指定をして画面をキャプチャ保存
```csharp
public static IEnumerator CaptureRect(string fileName, bool withTimestamp)
public static IEnumerator CaptureRect(string dirPath, string fileName, Rect range, bool withTimestamp)
```
