# CameraUtil

Provides camera related utility functions.

```csharp
namespace GarageKit
public class CameraUtil
```

#### Static Methods

Get camera from layer
```csharp
public static Camera FindCameraForLayer(int layer)
```

Get all camera list by depth
```csharp
public static List<Camera> GetCameraListByDepth()
```

Normalize screen coordinates with camera coordinates (-1.0 to 1.0)
```csharp
public static Vector3 NormalizeScreenPosition(Camera orthoCamera, Vector3 screenPosition)
```

Correct the coordinates when the Viewport goes off the screen
```csharp
public static Vector3 ViewportProtrusion(Vector3 viewportPosition, Vector2 ratio)
```