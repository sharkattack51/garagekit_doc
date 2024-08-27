# SevenTapLikeAndroid

Execute a callback by tapping seven times on a uGUI component, similar to the Android setting screen hidden operation.

```csharp
namespace GarageKit
public class SevenTapLikeAndroid : MonoBehaviour, IPointerDownHandler
```

#### Inheritance

`SevenTapLikeAndroid` -> `MonoBehaviour`, `IPointerDownHandler`

#### Methods

Callback for 7 consecutive taps
```csharp
public Action OnSevenTap
```

#### Example

- /Scenes/Examples/EventExample.unity
