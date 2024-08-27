# LineObject

平面方向を設定してターゲットオブジェクトまでのラインを引きます。ライン表現のために平面オブジェクトを子供階層に設置してください。

```csharp
namespace GarageKit
[ExecuteInEditMode]
public class LineObject : MonoBehaviour
```

#### Inheritance

`LineObject` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/lineobject_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|dimension|DIMENSION|平面方向設定|
|target|GameObject|ターゲットの参照|
|thickness|float|線の太さ|

#### Enums

##### __DIMENSION__

|enums|description|
|:--|:--|
|XY|XY 平面|
|XZ|XZ 平面|
