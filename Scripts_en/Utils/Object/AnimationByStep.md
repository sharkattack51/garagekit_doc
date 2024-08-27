# AnimationByStep

Step through the Animation component.

```csharp
namespace GarageKit
public class AnimationByStep : MonoBehaviour
```

#### Inheritance

`AnimationByStep` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/animationbystep_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|anim|Animation|Animation reference|
|speed|float|Step playback speed|
|useSmooth|bool|Use smooth update|

#### Methods

Step through animation
```csharp
public void Step()
```

Reset animation
```csharp
public void Reset()
```

Set animation position
```csharp
public void SetSeconds(float sec)
```

Get animation position
```csharp
public float GetSeconds()
```

Get animation duration
```csharp
public float GetDuration()
```
