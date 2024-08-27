# WindowsUtil

Provides Windows related utility functions.

```csharp
namespace GarageKit
public class WindowsUtil
```

#### Static Methods

Get the Rect of the application window
```csharp
public static Rect GetApplicationWindowRect()
```

Bring the application window to the foreground
```csharp
public static void SetForeGroundApplicationWindow()
```

Set application window to popup
```csharp
public static void SetPopupWindow()
```

Set application window position
```csharp
public static void SetWindowPos(int x, int y, int w, int h)
```

Minimize the specified application window
```csharp
public static void MinimizeWindow(string className, string windowName)
```

Minimize the application window
```csharp
public static void MinimizeWindow()
```

Maximize the specified application window
```csharp
public static void MaximizeWindow(string className, string windowName)
```

Maximize the application window
```csharp
public static void MaximizeWindow()
```
