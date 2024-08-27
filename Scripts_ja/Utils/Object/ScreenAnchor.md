# ScreenAnchor

スクリーン上の基準位置を指定して位置固定します。

```csharp
namespace GarageKit
public class ScreenAnchor : MonoBehaviour
```

#### Inheritance

`ScreenAnchor` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/screenanchor_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|anchorPosH|[ANCHOR_POSITION_HORIZONTAL](#anchor_position_horizontal)|横方向位置設定|
|anchorPosV|[ANCHOR_POSITION_VERTICAL](#anchor_position_vertical)|縦方向位置設定|
|useUpdateAnchor|bool|固定処理を Update() で行う|

#### Enums

##### __ANCHOR_POSITION_HORIZONTAL__

|enums|description|
|:--|:--|
|LEFT|左端|
|MIDDLE|中央|
|RIGHT|右端|

##### __ANCHOR_POSITION_VERTICAL__

|enums|description|
|:--|:--|
|TOP|上端|
|MIDDLE|中央|
|BOTTOM|下端|
