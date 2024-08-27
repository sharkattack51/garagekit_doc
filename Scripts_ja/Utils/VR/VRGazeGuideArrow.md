# VRGazeGuideArrow

VR での視線ガイド矢印を表示コントロールします。

```csharp
namespace GarageKit
public class VRGazeGuideArrow : MonoBehaviour
```

#### Inheritance

`VRGazeGuideArrow` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/vrgazeguidearrow_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|viewCamera|Camera|HMD カメラの参照|
|smoothTime|float|スムーズ移動量|
|screenRatio|float|ガイドが有効になるスクリーン範囲|
|arrows|GameObject[]|矢印オブジェクト|
|modeGreen|Color32|グリーンモードカラー|
|modeRed|Color32|レッドモードカラー|
|useArrow|bool|矢印表示設定|

#### Enums

##### __COLOR_MODE__

|enums|description|
|:--|:--|
|GREEN|グリーンモード|
|RED|レッドモード|

#### Methods

HMD デバイスの利用中確認
```csharp
public bool IsDevicePresent()
```

カラーモードの切り替え
```csharp
public void ChangeColor(COLOR_MODE mode)
```
