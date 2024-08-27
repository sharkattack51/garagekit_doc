# ARKitCoachingOverlay

Controls the coaching view of iOS ARKit's native functionality.
https://developer.apple.com/documentation/arkit/arcoachingoverlayview

> [!IMPORTANT]
> When using it, please enable #define definition in the source code.

```csharp
namespace GarageKit.ARFoundationExtention
[RequireComponent(typeof(ARSession))]
public class ARKitCoachingOverlay : MonoBehaviour
```

#### Inheritance

`ARKitCoachingOverlay` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arkitcoachingoverlay_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|Goal|CoachingGoal|Goals to direct tracking requirements|
|ActivatesAutomatically|bool|auto enable|

#### Enums

##### __CoachingGoal__

|enums|description|
|:--|:--|
|Tracking|World tracking|
|HorizontalPlane|Horizontal plane tracking|
|VerticalPlane|Vertical plane tracking|
|AnyPlane|Any plane tracking|

#### Methods

Check support for coaching function
```csharp
public bool supported { get; }
```

Enabling coaching
```csharp
public void ActivateCoaching(bool animated)
```

Disabling coaching
```csharp
public void DisableCoaching(bool animated) 
```
