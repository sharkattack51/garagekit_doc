# SequenceSprite

Switch sequential number Sprites in frames.

```csharp
namespace GarageKit
public class SequenceSprite : MonoBehaviour
```

#### Inheritance

`SequenceSprite` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/sequencesprite_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiImage|Image|Image reference|
|sprites|Sprite[]|Sequential sprite|

#### Methods

Reset sequence
```csharp
public void ResetSequence()
```

Start sequence
```csharp
public void StartSequence()
```

Stop sequence
```csharp
public void StopSequence()
```
