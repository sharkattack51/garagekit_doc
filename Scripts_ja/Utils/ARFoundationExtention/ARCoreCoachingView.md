# ARCoreCoachingView

Android ARCore 利用時に iOS ARKit のコーチングビュー表示を真似て表示できます。

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

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
|planeManager|ARPlaneManager|ARPlaneManager の参照|
|view|CanvasGroup|View グループ|

#### Methods

View の有効化
```csharp
public void ActivateCoaching()
```

View の無効化
```csharp
public void DisableCoaching()
```
