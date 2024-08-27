# FpsCounter

uGUI による簡易的な FPS 表示を行います。([Graphy](https:/assetstore.unity.com/packages/tools/gui/graphy-ultimate-fps-counter-stats-monitor-debugger-105778?locale=ja-JP) の利用をお勧めします)

<img src="~/image/script_reference/fpscounter_gameview.png" width="500px"/>
</br>
</br>

```csharp
namespace GarageKit
public class FpsCounter : MonoBehaviour
```

#### Inheritance

`FpsCounter` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/fpscounter_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|displayFPS|bool|表示設定|
|text|Text|Text コンポーネントの参照|
|targetFPS|int|ターゲット FPS|
|goodColor|Color|Good 時カラー|
|warnColor|Color|Warn 時カラー|
|badColor|Color|Bad 時カラー|
