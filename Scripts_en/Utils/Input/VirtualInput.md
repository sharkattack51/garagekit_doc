# VirtualInput

Executes operations by emulating keyboard and mouse operations in Windows.

```csharp
namespace GarageKit
public class VirtualInput
```

#### Static Methods

Keyboard input
```csharp
public static void KeyDown(int keyCode)
public static void KeyDown(int keyCode1, int keyCode2)
public static void KeyDown(int keyCode1, int keyCode2, int keyCode3)
```

Mouse move
```csharp
public static void MouseMove(int posX, int posY)
```

Mouse click
```csharp
public static void MouseClick(int posX, int posY)
```

mouse double click
```csharp
public static void MouseDoubleClick(int posX, int posY)
```

#### Example

```csharp
// A key input
VirtualInput.KeyDown(KeyCode.VK_A);

// SHIFT + B key input
VirtualInput.KeyDown(KeyCode.VK_L_SHIFT, KeyCode.VK_B);

// Mouse move and click
float x = Screen.Width / 2.0f;
float y = Screen.Height / 2.0f;
VirtualInput.MouseMove(x, y);
VirtualInput.MouseClick(x, y);
```

---

# KeyCode

Key code information structure

#### Properties

http://msdn.microsoft.com/ja-jp/library/windows/desktop/dd375731(v=vs.85).aspx

```csharp
public const int VK_L_SHIFT = 0x00A0;
public const int VK_R_SHIFT = 0x00A1;
public const int VK_L_CONTROL = 0x00A2;
public const int VK_R_CONTROL = 0x00A3;
public const int VK_BACKSPACE = 0x0008;
public const int VK_TAB = 0x0009;
public const int VK_RETURN = 0x000D;
public const int VK_ALT = 0x0012;
public const int VK_ESCAPE = 0x001B;
public const int VK_SPACE = 0x0020;
public const int VK_LEFT_ARROW = 0x0025;
public const int VK_UP_ARROW = 0x0026;
public const int VK_RIGHT_ARROW = 0x0027;
public const int VK_DOWN_ARROW = 0x0028;
public const int VK_DELETE = 0x002E;

public const int VK_0 = 0x0030;	
public const int VK_1 = 0x0031;	
public const int VK_2 = 0x0032;	
public const int VK_3 = 0x0033;	
public const int VK_4 = 0x0034;	
public const int VK_5 = 0x0035;	
public const int VK_6 = 0x0036;	
public const int VK_7 = 0x0037;	
public const int VK_8 = 0x0038;	
public const int VK_9 = 0x0039;	

public const int VK_A = 0x0041;
public const int VK_B = 0x0042;
public const int VK_C = 0x0043;
public const int VK_D = 0x0044;
public const int VK_E = 0x0045;
public const int VK_F = 0x0046;
public const int VK_G = 0x0047;
public const int VK_H = 0x0048;
public const int VK_I = 0x0049;
public const int VK_J = 0x004A;
public const int VK_K = 0x004B;
public const int VK_L = 0x004C;
public const int VK_M = 0x004D;
public const int VK_N = 0x004E;
public const int VK_O = 0x004F;
public const int VK_P = 0x0050;
public const int VK_Q = 0x0051;
public const int VK_R = 0x0052;
public const int VK_S = 0x0053;
public const int VK_T = 0x0054;
public const int VK_U = 0x0055;
public const int VK_V = 0x0056;
public const int VK_W = 0x0057;
public const int VK_X = 0x0058;
public const int VK_Y = 0x0059;
public const int VK_Z = 0x005A;

public const int VK_NUM_0 = 0x0060;
public const int VK_NUM_1 = 0x0061;
public const int VK_NUM_2 = 0x0062;
public const int VK_NUM_3 = 0x0063;
public const int VK_NUM_4 = 0x0064;
public const int VK_NUM_5 = 0x0065;
public const int VK_NUM_6 = 0x0066;
public const int VK_NUM_7 = 0x0067;
public const int VK_NUM_8 = 0x0068;
public const int VK_NUM_9 = 0x0069;

public const int VK_F1 = 0x0070;
public const int VK_F2 = 0x0071;
public const int VK_F3 = 0x0072;
public const int VK_F4 = 0x0073;
public const int VK_F5 = 0x0074;
public const int VK_F6 = 0x0075;
public const int VK_F7 = 0x0076;
public const int VK_F8 = 0x0077;
public const int VK_F9 = 0x0078;
public const int VK_F10 = 0x0079;
public const int VK_F11 = 0x007A;
public const int VK_F12 = 0x007B;

public const int VK_L_WINDOWS = 0x005B;
public const int VK_R_WINDOWS = 0x005C;
```
