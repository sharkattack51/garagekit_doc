# TimerEvent

カウントダウンのタイマーで時間によるイベントを設定できます。

```csharp
namespace GarageKit
public class TimerEvent : MonoBehaviour
```

#### Inheritance

`TimerEvent` -> `MonoBehaviour`

#### Methods

タイマー開始済み確認
```csharp
public bool IsStarted { get; }
```

タイマー実行中確認
```csharp
public bool IsRunning { get; }
```

タイマー残り時間（秒）
```csharp
public int CurrentTime { get; }
```

タイマー経過時間（秒）
```csharp
public float ElapsedTime { get; }
```

タイマー毎秒経過イベント
```csharp
public event OnTimerDelegate OnTimer
```

タイマー完了イベント
```csharp
public event OnCompleteTimerDelegate OnCompleteTimer
```

タイマーの開始
```csharp
public void StartTimer(int countTime, float delayTime = 0.0f, bool autoDestroy = false)
```

タイマーの停止
```csharp
public void StopTimer()
```

タイマーの一時停止
```csharp
public void ResumeTimer()
```

タイマーのリセット
```csharp
public void ResetTimer(bool andStart)
```

#### Example

- /Scenes/Examples/EventExample.unity

```csharp
GameObject obj = new GameObject("TimerEventObject"); 
obj.AddComponent<TimerEvent>();
obj.GetComponent<TimerEvent>().OnTimer += (sender, sec) => {};
obj.GetComponent<TimerEvent>().OnCompleteTimerEvent += (sender) => {};
obj.GetComponent<TimerEvent>().StartTimer(10); // count down 10 sec
```
