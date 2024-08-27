# UserInputManager

Manage user input functionality. It is convenient to collect all user input code here.

```csharp
namespace GarageKit
public class UserInputManager : ManagerBase
```

#### Inheritance

`UserInputManager` -> [ManagerBase](../Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Example

Default implemented key:

|Key|Function|
|:--|:--|
|Esc|Quit application|
|D|Toggle debugging features|
|R|Reload ApplicationSetting.xml|
|Backspace|Capture the current GameView and save the image to the desktop|
