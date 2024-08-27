# Win10VirtualKeyboard

Windows 10 の OS 標準ソフトウェアキーボードを表示制御します。InputField 上のテキスト入力操作を制御するために Update() での監視を行なっているので、GameObject インスタンスとして利用します。

```csharp
namespace GarageKit
public class Win10VirtualKeyboard : MonoBehaviour
```

#### Inheritance

`Win10VirtualKeyboard` -> `MonoBehaviour`

#### Static Methods

ソフトウェアキーボード(`tabtip.exe`)を表示する
```csharp
public static void ShowTouchKeyboard()
```

ソフトウェアキーボード(`tabtip.exe`)を非表示にする
```csharp
public static void HideTouchKeyboard()
```

ソフトウェアキーボード(`OSK`)を表示する
```csharp
public static void ShowOnScreenKeyboard()
```

ソフトウェアキーボード(`OSK`)を非表示にする
```csharp
public static void HideOnScreenKeyboard()
```

ソフトウェアキーボード(`OSK`)の表示位置を変更
```csharp
public static void RepositionOnScreenKeyboard(Rect rect)
```
