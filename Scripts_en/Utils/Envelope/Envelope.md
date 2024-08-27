# Envelope

Create animation curves dynamically at runtime from the keyframe data list.

```csharp
namespace GarageKit
public class Envelope : MonoBehaviour
```

#### Inheritance

`Envelope` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/envelope_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|propertyName|string|Identification property name|
|preWrapMode|WrapMode|Forward wrap mode|
|postWrapMode|WrapMode|Backward wrap mode|
|envelopeKeys|[EnvelopeKey](#envelopekey)[]|Keyframe data list|

#### Methods

Get animation curve
```csharp
public AnimationCurve GetCurve()
```

---

# EnvelopeKey

Keyframe data structure

```csharp
namespace GarageKit
[Serializable]
public class EnvelopeKey
```

#### Properties

|member|type|description|
|:--|:--|:--|
|time|float|Time X|
|value|float|Value Y|
|leftTangent|AnimationCurveUtil.TangentMode|Left handle tangent|
|rightTangent|AnimationCurveUtil.TangentMode|Right handle tangent|
