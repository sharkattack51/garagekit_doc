# LineObject

Set the plane direction and draw a line to the target object. Place a plane object in the child hierarchy for line expression.

```csharp
namespace GarageKit
[ExecuteInEditMode]
public class LineObject : MonoBehaviour
```

#### Inheritance

`LineObject` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/lineobject_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|dimension|DIMENSION|Plane direction setting|
|target|GameObject|Target reference|
|thickness|float|Line thickness|

#### Enums

##### __DIMENSION__

|enums|description|
|:--|:--|
|XY|XY plane|
|XZ|XZ plane|
