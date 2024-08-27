# AutoUVScroll

UVの自動スクロールアニメーションをします。

```csharp
namespace GarageKit
public class AutoUVScroll : MonoBehaviour
```

#### Inheritance

`AutoUVScroll` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/autouvscroll_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|materialID|int|マテリアル番号|
|texturePropName|string|シェーダーのテクスチャプロパティ名|
|scrollTime|float|スクロールアニメーション時間|
|startUV|Vector2|開始点の UV 値|
|endUV|Vector2|終点の UV 値|
|easeType|Ease|イージングタイプ|
|loopType|LoopType|ループタイプ|
