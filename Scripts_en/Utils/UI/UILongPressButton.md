# UILongPressButton

Button component that can be executed by long press.

```csharp
namespace GarageKit
[RequireComponent(typeof(EventTrigger))]
public class UILongPressButton : MonoBehaviour
```

#### Inheritance

`UILongPressButton` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/uilongpressbutton_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|holdTime|float|Long press time|

#### Methods

Long press execution callback
```csharp
public Action OnHoldButton
```
