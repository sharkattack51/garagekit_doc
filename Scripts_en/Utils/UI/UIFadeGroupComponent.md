# UIFadeGroupComponent

Manages fade processing for a CanvasGroup.

```csharp
namespace GarageKit
public class UIFadeGroupComponent : MonoBehaviour
```

#### Inheritance

`UIFadeGroupComponent` -> `MonoBehaviour`

#### Methods

Reset fade
```csharp
public void ResetFade()
```

Start fade
```csharp
public void StartFade(float fixTime = 5.0f, float tweenTime = 0.5f)
```

Set UI position by distance to camera position
```csharp
public void SetUiPosition3D(Vector3 camPos, Vector3 targetPos, float height = 1.8f, float depth = 1.5f)
```
