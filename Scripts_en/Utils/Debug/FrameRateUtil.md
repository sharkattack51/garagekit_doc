# FrameRateUtil

Performs a simple FPS display using OnGUI(). (Recommend using [Graphy](https:/assetstore.unity.com/packages/tools/gui/graphy-ultimate-fps-counter-stats-monitor-debugger-105778))

<img src="~/image/script_reference/framerateutil_gameview.png" width="500px"/>
</br>
</br>

```csharp
namespace GarageKit
public class FrameRateUtil : MonoBehaviour
```

#### Inheritance

`FrameRateUtil` -> `MonoBehaviour`

#### Properties

|member|type|description|
|:--|:--|:--|
|useHUD|bool|Display settings|

#### Static Methods

Get current FPS value
```csharp
public static float Fps { get; }
```
