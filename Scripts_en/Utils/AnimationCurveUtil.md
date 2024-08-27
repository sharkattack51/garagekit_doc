# AnimationCurveUtil

Provides utility functions related to animation curve settings.

reference: UnityEditor.CurveUtility.cs (c) Unity Technologies

```csharp
namespace GarageKit
public class AnimationCurveUtil
```

#### Static Methods

Set animation curve interpolation to linear
```csharp
public static void UpdateAllLinearTangents(AnimationCurve curve)
```

Tangent mode update of animation curve specified keyframe
```csharp
public static void UpdateTangentsFromMode(AnimationCurve curve, int index)
```

Generating and acquiring new keyframes
```csharp
public static Keyframe GetNewKey(float time, float value, TangentMode leftAndRight)
public static Keyframe GetNewKey(float time, float value, TangentMode left, TangentMode right)
```

Get keyframe tangent mode
```csharp
public static TangentMode GetKeyTangentMode(int tangentMode, int leftRight)
public static TangentMode GetKeyTangentMode(Keyframe keyframe, int leftRight)
```

Disconnect the left and right handles of the key frame
```csharp
public static void SetKeyBroken(object keyframe, bool broken)
```

#### Enums

##### __TangentMode__

|enums|description|
|:--|:--|
|Editable|custom interpolation|
|Smooth|smooth curve interpolation|
|Linear|liner line interpolation|
|Stepped|step interpolation|
