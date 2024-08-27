# FrameRateUtil

MonoBehaviour.OnGUI() による簡易的な FPS 表示を行います。([Graphy](https:/assetstore.unity.com/packages/tools/gui/graphy-ultimate-fps-counter-stats-monitor-debugger-105778?locale=ja-JP) の利用をお勧めします)

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
|useHUD|bool|表示設定|

#### Static Methods

現在の FPS 値の取得
```csharp
public static float Fps { get; }
```
