# NumberTexture

Set and switch textures from the input values ​​0-9.

```csharp
namespace GarageKit
public class NumberTexture : MonoBehaviour
```

#### Inheritance

`NumberTexture` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/numberexture_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|numTextures|Texture2D[]|Number texture 0-9|
|numPlates|GameObject[]|Digit object starting with the ones digit|

#### Methods

Set number texture
```csharp
public void SetNumber(int num)
```
