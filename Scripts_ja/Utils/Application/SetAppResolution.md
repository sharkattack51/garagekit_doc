# SetAppResolution

解像度設定をインスペクタから行います。

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
|resolutionType|[APP_RESOLUTION](#app_resolution)|解像度タイプ設定|
|fullScreen|bool|フルスクリーン設定|
|resolutionID|int|ディスプレイ対応解像度指定時の ID|
|customWindowRect|Vector4|カスタムタイプ時のウィンドウ位置解像度|
|useFixAspect|bool|アスペクト比固定設定|
|aspectRatio|float|アスペクト比|

#### Enums

##### __APP_RESOLUTION__

|enums|description|
|:--|:--|
|PLAYER_SETTINGS_RESOLUTIOM|プレイヤー設定で行う|
|CURRENT_FULLSCREEN|現在のフルスクリーン|
|DISPLAY_SUPPORTED|ディスプレイ対応解像度指定|
|CUSTOM_RESOLUTION|解像度指定|
|CUSTOM_RESOLUTION_POPUPWINDOW|ポップアップウィンドウでの解像度指定|
