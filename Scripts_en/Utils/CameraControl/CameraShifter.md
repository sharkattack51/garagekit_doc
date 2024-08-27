# CameraShifter

Perform camera shift. The camera FOV setting will have no effect as the projectionMatrix will be overwritten internally.

```csharp
namespace GarageKit
public class CameraShifter
```

#### Inheritance

`CameraShifter` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/camerashifter_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|shiftX|float|Percentage of horizontal shift|
|shiftY|float|Percentage of vertical shift|
|calcAlways|bool|Update with Update() or not|

#### Methods

Reset to initial state
```csharp
public void ResetProjMat()
```
