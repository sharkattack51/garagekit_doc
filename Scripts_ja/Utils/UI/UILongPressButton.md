# UILongPressButton

長押しで実行できるボタンコンポーネント

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
|holdTime|float|長押しする時間|

#### Methods

長押しでの実行コールバック
```csharp
public Action OnHoldButton
```
