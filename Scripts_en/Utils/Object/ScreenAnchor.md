# ScreenAnchor

Specify the reference position on the screen and fix the position.

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
|anchorPosH|[ANCHOR_POSITION_HORIZONTAL](#anchor_position_horizontal)|Horizontal position setting|
|anchorPosV|[ANCHOR_POSITION_VERTICAL](#anchor_position_vertical)|Vertical position setting|
|useUpdateAnchor|bool|Perform fixed processing with Update()|

#### Enums

##### __ANCHOR_POSITION_HORIZONTAL__

|enums|description|
|:--|:--|
|LEFT|Left edge|
|MIDDLE|Horizontal center|
|RIGHT|Right wdge|

##### __ANCHOR_POSITION_VERTICAL__

|enums|description|
|:--|:--|
|TOP|Top edge|
|MIDDLE|Vertical center|
|BOTTOM|Bottom edge|
