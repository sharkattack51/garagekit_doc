# AppMain

A singleton instance that is responsible for the reference route to each manager.

```csharp
namespace GarageKit
public class AppMain : MonoBehaviour
```

#### Inheritance

`AppMain` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/appmain_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|asDontDestroyOnLoad|bool|When used in multiple scenes, it is shared between scenes without being discarded when moving scenes.|

#### Static Methods

Get a singleton instance
```csharp
public static AppMain Instance { get; }
```

#### Example

```csharp
// Routing to each manager
AppMain.Instance.sceneStateManager.ChangeState("PLAY");
AppMain.Instance.soundManager.Play("SE", "CLICK");
```
