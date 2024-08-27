# GyroCamera

Operate camera rotation with gyro.

> [!IMPORTANT]
> When using the GyroDroid package, please enable #define definition in the source code.

```csharp
namespace GarageKit
public class GyroCamera
```

#### Inheritance

`GyroCamera` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/gyrocamera_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|northDirection|[NORTH_DIRECTION](#north_direction)|Setting the reference direction (north)|

#### Enums

##### __NORTH_DIRECTION__

|enums|description|
|:--|:--|
|NONE|none|
|COMPASS_NORTH|North direction of compass|
|GYRO_HEAD_DIRECTION|Z direction|

#### Methods

Check preparation completed
```csharp
public bool IsReady { get; }
```

Callback when ready
```csharp
public Action OnReady
```

Set current Z to reference direction (north)
```csharp
public void CalibrateNorth()
```

Change camera FOV
```csharp
public void SetFov(float fov)
```
