# SequenceSprite

フレームで連番 Sprite を切り替えます。

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
|uiImage|Image|Image の参照|
|sprites|Sprite[]|連番 Sprite|

#### Methods

連番のリセット
```csharp
public void ResetSequence()
```

連番の切り替え開始
```csharp
public void StartSequence()
```

連番の切り替え停止
```csharp
public void StopSequence()
```
