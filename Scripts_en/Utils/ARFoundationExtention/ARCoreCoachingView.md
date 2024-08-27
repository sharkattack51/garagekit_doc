# ARCoreCoachingView

When using Android ARCore, you can imitate iOS ARKit's coaching view display.

> [!IMPORTANT]
> When using it, please enable #define definition in the source code.

```csharp
namespace GarageKit.ARFoundationExtention
public class ARCoreCoachingView : MonoBehaviour
```

#### Inheritance

`ARCoreCoachingView` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arcorecoachingview_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|planeManager|ARPlaneManager|ARPlaneManager reference|
|view|CanvasGroup|View group|

#### Methods

Enabling view
```csharp
public void ActivateCoaching()
```

Disabling view
```csharp
public void DisableCoaching()
```
