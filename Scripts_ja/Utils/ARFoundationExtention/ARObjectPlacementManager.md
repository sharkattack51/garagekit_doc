# ARObjectPlacementManager

タッチ入力での ARRaycastHit によって AR オブジェクトを配置固定します。

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit.ARFoundationExtention
public class ARObjectPlacementManager : MonoBehaviour
```

#### Inheritance

`ARObjectPlacementManager` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arobjectplacementmanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|raycastManager|ARRaycastManager|ARRaycastManager の参照|
|isInstantiate|bool|インスタンス配置の有効化|
|instantiateRef|GameObject|インスタンス化元のプレハブ|
|touchBlockers|RectTransform[]|タッチ入力判定をブロックする UI オブジェクトリスト|

#### Methods

最後に配置した AR オブジェクトの参照
```csharp
public IPlacableObject PlacableObj { get; }
```

---

# IPlacableObject

配置する AR オブジェクトのインターフェース

```csharp
namespace GarageKit.ARFoundationExtention
public interface IPlacableObject
```

#### Methods

配置時に SendMessage で呼ばれるコールバック
```csharp
void OnPlace();
```
