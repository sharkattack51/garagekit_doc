# Win10VirtualKeyboard

Controls the display of the Windows 10 OS standard software keyboard. Since we are monitoring with Update() to control the text input operation on the InputField, we will use it as a GameObject instance.

```csharp
namespace GarageKit
public class Win10VirtualKeyboard : MonoBehaviour
```

#### Inheritance

`Win10VirtualKeyboard` -> `MonoBehaviour`

#### Static Methods

Display software keyboard (`tabtip.exe`)
```csharp
public static void ShowTouchKeyboard()
```

Hide software keyboard (`tabtip.exe`)
```csharp
public static void HideTouchKeyboard()
```

Display software keyboard (`OSK`)
```csharp
public static void ShowOnScreenKeyboard()
```

Hide software keyboard (`OSK`)
```csharp
public static void HideOnScreenKeyboard()
```

Change the display position of the software keyboard (`OSK`)
```csharp
public static void RepositionOnScreenKeyboard(Rect rect)
```
