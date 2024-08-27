# OnRenderHandler

Run the MonoBehaviour's OnPreRender() and OnPostRender() functions in a callback.

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
