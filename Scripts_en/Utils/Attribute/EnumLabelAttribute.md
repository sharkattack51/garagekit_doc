# EnumLabelAttribute

Add a `[Label("label name")]` attribute to each value of an enum type to obtain a label string separate from the value.

```csharp
namespace GarageKit
public class EnumAttribute
```

#### Methods

Get label string
```csharp
public static string LabelAttribute(this Enum value)
```

Get label string array
```csharp
 public static string[] LabelAttributes<T>() where T : Enum
```

#### Example

```csharp
enum TIER_TYPE
{
    [Label("UP")]
    UPPER = 0,

    [Label("MID")]
    MIDDLE,

    [Label("BTM")]
    BOTTOM
}

// Get the label name from the value of an enum object
string label = TIER_TYPE.UPPER.LabelAttribute(); // "UP"

// Get the label name array from a declared enum type
string[] labels = EnumLabelAttribute.LabelAttributes<TIER_TYPE>(); // [ "UP", "MID", "BTM" ]
```
