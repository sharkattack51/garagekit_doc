# StandalonePlayerResolutionHelper

Removes the resolution settings that are automatically saved in the registry when Windows StandalonePlayer runs to avoid an issue where it runs at the wrong resolution the next time it starts.

> [!IMPORTANT]
> It is not used on anything other than Windows.

> [!IMPORTANT]
> If you want to use it, change ApiCompatibilityLevel in PlayerSettings to `.NET Framework`.

```csharp
namespace GarageKit
[ExecuteInEditMode]
public class StandalonePlayerResolutionHelper : MonoBehaviour
```

#### Inheritance

`StandalonePlayerResolutionHelper` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/standaloneplayerresolutionhelper_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|playerSettingsCompanyName|string|CompanyName in player settings|
|playerSettingsProductName|string|ProductName in player settings|

> [!IMPORTANT]
> Since it is executed in OnApplicationQuit(), it will not be deleted from the registry unless it terminates normally, such as by a process Kill or Shutdown command.

