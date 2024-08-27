# Billbord

指定ターゲットオブジェクトに対してビルボード処理を実行します。

```csharp
namespace GarageKit
public class Billbord : MonoBehaviour
```

#### Inheritance

`Billbord` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/billbord_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|target|Transform|ターゲットの参照|
|invertForward|bool|前方向を反転|
|invertUp|bool|上方向を反転|
|lockPitch|bool|ピッチ回転をしない|
|isZup|bool|Z 軸を上方向にする|
|asGroup|bool|グループとして子供階層全オブジェクトに反映|
