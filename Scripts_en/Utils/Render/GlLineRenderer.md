# GlLineRenderer

OnPostRender() draws a GL line at the specified coordinates.

```csharp
namespace GarageKit
[RequireComponent(typeof(Camera))]
public class GlLineRenderer : MonoBehaviour
```

#### Inheritance

`GlLineRenderer` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/gllinerenderer_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|lineColor|Color|Drawing line color|
|lines|[LineData](#linedata)[]|Drawing line coordinate list|
|lineMaterial|Material|Drawing material|

#### Methods

Update line coordinates
```csharp
public void UpdateLine(int id, Vector2 start, Vector2 end)
```

---

# LineData

Structure of drawing line coordinates

```csharp
namespace GarageKit
[Serializable]
public class LineData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|start|Vector2|Start point|
|end|Vector2|End point|
