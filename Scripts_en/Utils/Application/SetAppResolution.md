# SetAppResolution

Set the resolution from the inspector.

```csharp
namespace GarageKit
public class SetAppResolution : MonoBehaviour
```

#### Inheritance

`SetAppResolution` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/setappresolution_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|resolutionType|[APP_RESOLUTION](#app_resolution)|Resolution type setting|
|fullScreen|bool|full screen settings|
|resolutionID|int|ID when specifying display resolution|
|customWindowRect|Vector4|Window position resolution when custom type|
|useFixAspect|bool|Fixed aspect ratio setting|
|aspectRatio|float|aspect ratio|

#### Enums

##### __APP_RESOLUTION__

|enums|description|
|:--|:--|
|PLAYER_SETTINGS_RESOLUTIOM|Depends on player settings|
|CURRENT_FULLSCREEN|Current full screen|
|DISPLAY_SUPPORTED|Resolutions supported display|
|CUSTOM_RESOLUTION|Resolution specification|
|CUSTOM_RESOLUTION_POPUPWINDOW|Specifying resolution in popup window|
