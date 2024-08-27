# SevenTapLikeAndroid

Android の設定画面隠し操作のように、uGUI のコンポーネント上で 7 回連続タップ操作でコールバックの実行をします。

```csharp
namespace GarageKit
public class SevenTapLikeAndroid : MonoBehaviour, IPointerDownHandler
```

#### Inheritance

`SevenTapLikeAndroid` -> `MonoBehaviour`, `IPointerDownHandler`

#### Methods

7 回連続タップ時のコールバック
```csharp
public Action OnSevenTap
```

#### Example

- /Scenes/Examples/EventExample.unity
