# OnRenderHandler

MonoBehaviour の OnPreRender() と OnPostRender() 関数をコールバック化して実行します。

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class OnRenderHandler : MonoBehaviour
```

#### Inheritance

`OnRenderHandler` -> `MonoBehaviour`

#### Methods

```csharp
public Action OnPreRenderAction
```

```csharp
public Action OnPostRenderAction
```
