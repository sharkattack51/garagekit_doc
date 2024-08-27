# VRSceneStateBase

[SceneStateManager](~/Scripts_en/Managers/SceneStateManager.md) Interface for performing state transition for VR content.

```csharp
namespace GarageKit
public interface VRSceneStateBase
```

#### Methods

Implementation of processing to reset the current state
```csharp
void ResetCurrentState()
```

Implementation of display object setting processing
```csharp
void SetStagingObjects();
```
