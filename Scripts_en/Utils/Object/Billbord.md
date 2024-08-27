# Billbord

Executes billboard processing on the specified target object.

```csharp
namespace GarageKit
public class Billbord : MonoBehaviour
```

#### Inheritance

`Billbord` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/billbord_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|target|Transform|Target reference|
|invertForward|bool|Reverse front direction|
|invertUp|bool|Reverse up direction|
|lockPitch|bool|No pitch rotation|
|isZup|bool|Z axis is upward|
|asGroup|bool|All objects in the child hierarchy are reflected|
