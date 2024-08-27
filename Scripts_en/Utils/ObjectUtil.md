# ObjectUtil

Provides utility functions related to object manipulation.

```csharp
namespace GarageKit
public class ObjectUtil
```

#### Static Methods

Setting layers of child hierarchy objects all at once
```csharp
public static void SetLayerChildren(GameObject rootObject, int layer, bool changeParent = false)
```

Get the bounding box of the entire hierarchy
```csharp
public static Bounds GetRenderBoundsChildren(GameObject root)
```
