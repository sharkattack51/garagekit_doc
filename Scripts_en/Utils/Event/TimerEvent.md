# TimerEvent

Set events based on time with a countdown timer.

```csharp
namespace GarageKit
public class TimerEvent : MonoBehaviour
```

#### Inheritance

`TimerEvent` -> `MonoBehaviour`

#### Methods

Check if the timer has started
```csharp
public bool IsStarted { get; }
```

Check if timer is running
```csharp
public bool IsRunning { get; }
```

Timer remaining time (seconds)
```csharp
public int CurrentTime { get; }
```

Timer elapsed time (seconds)
```csharp
public float ElapsedTime { get; }
```

Timer elapsed event per second
```csharp
public event OnTimerDelegate OnTimer
```

Timer completion event
```csharp
public event OnCompleteTimerDelegate OnCompleteTimer
```

Start timer
```csharp
public void StartTimer(int countTime, float delayTime = 0.0f, bool autoDestroy = false)
```

Stop timer
```csharp
public void StopTimer()
```

Resume timer
```csharp
public void ResumeTimer()
```

Reset timer
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
