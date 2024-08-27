# ZsortOrderGroup

子供階層の全オブジェクトをターゲットからの距離順でソートします。

```csharp
namespace GarageKit
public class ZsortOrderGroup : MonoBehaviour
```

#### Inheritance

`WebCamPlateObject` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/zsortordergroup_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|distanceTarget|Transform|距離判定用のターゲット|
|isReverse|bool|ソート順を逆転|
