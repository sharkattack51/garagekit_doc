# ARObjectPlacementManager

Place AR object by ARRaycastHit on touch input.

> [!IMPORTANT]
> When using it, please enable #define definition in the source code.

```csharp
namespace GarageKit.ARFoundationExtention
public class ARObjectPlacementManager : MonoBehaviour
```

#### Inheritance

`ARObjectPlacementManager` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arobjectplacementmanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|raycastManager|ARRaycastManager|ARRaycastManager reference|
|isInstantiate|bool|Enabling instance placement|
|instantiateRef|GameObject|Prefab to instantiate from|
|touchBlockers|RectTransform[]|UI object list that blocks touch input judgment|

#### Methods

Reference to last placed AR object
```csharp
public IPlacableObject PlacableObj { get; }
```

---

# IPlacableObject

Interface of AR object to place

```csharp
namespace GarageKit.ARFoundationExtention
public interface IPlacableObject
```

#### Methods

Callback called by SendMessage
```csharp
void OnPlace();
```
