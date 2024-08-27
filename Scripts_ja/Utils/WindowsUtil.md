# WindowsUtil

Windows 関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class WindowsUtil
```

#### Static Methods

アプリケーションウィンドウの Rect を取得
```csharp
public static Rect GetApplicationWindowRect()
```

アプリケーションウィンドウを前景にする
```csharp
public static void SetForeGroundApplicationWindow()
```

アプリケーションウィンドウをポップアップに設定する
```csharp
public static void SetPopupWindow()
```

アプリケーションウィンドウの位置を設定する
```csharp
public static void SetWindowPos(int x, int y, int w, int h)
```

指定したアプリケーションウィンドウを最小化する
```csharp
public static void MinimizeWindow(string className, string windowName)
```

アプリケーションウィンドウを最小化する
```csharp
public static void MinimizeWindow()
```

指定したアプリケーションウィンドウを最大化する
```csharp
public static void MaximizeWindow(string className, string windowName)
```

アプリケーションウィンドウを最大化する
```csharp
public static void MaximizeWindow()
```
