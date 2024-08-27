# AutoRotate

オブジェクトの自動回転アニメーションをします。

```csharp
namespace GarageKit
public class AutoRotate : MonoBehaviour
```

#### Inheritance

`AutoRotate` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/autorotate_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|rotateSpeed|float|回転速度|
|axis|[ROTATE_AXIS](#rotate_axis)|回転軸|

#### Enums

##### __ROTATE_AXIS__

|enums|description|
|:--|:--|
|X|X 軸|
|Y|Y 軸|
|Z|Z 軸|
|XY|X 軸と Y 軸|
|XZ|X 軸と Z 軸|
|YZ|Y 軸と Z 軸|
|XYZ|全軸|
