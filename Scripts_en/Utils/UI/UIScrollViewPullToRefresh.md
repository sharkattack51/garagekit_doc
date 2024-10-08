# UIScrollViewPullToRefresh

Component for the function that pulls the scroll view down and refresh the content.

```csharp
namespace GarageKit
public class UIScrollViewPullToRefresh : MonoBehaviour
```

#### Inheritance

`UIScrollViewPullToRefresh` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/uiscrollviewpulltorefresh_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiScrlRect|ScrollRect|ScrollRect reference|
|indicatorImg|Image|Indicator image reference|

#### Methods

Callback to start pull down operation
```csharp
public Action OnPullStart
```

Callback for canceling pull down operation
```csharp
public Action OnPullCancel
```

Callback when the scroll threshold is exceeded by pulling down
```csharp
public Action OnPullOverTh
```

Callback when refreshing after finishing the pull down operation
```csharp
public Action OnPullToRefresh
```
