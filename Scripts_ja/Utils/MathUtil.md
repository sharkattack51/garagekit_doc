# MathUtil

数学関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class MathUtil
```

#### Static Methods

ローパスフィルター
```csharp
public static float LowPassFilter(float pre, float current, float weight = 0.05f)
```

---
# KalmanFilter

カルマンフィルター https://garchiving.com/gyro-drift-correction/

```csharp
namespace GarageKit.MathUtil
public class KalmanFilter
```

#### Methods

```csharp
public float GetAngle(float newAngle, float newRate, float dt)
```

```csharp
public void SetAngle(float angle)
```

```csharp
public float GetRate()
```

```csharp
public void SetQangle(float Q_angle)
```

```csharp
public void SetQbias(float Q_bias)
```

```csharp
public float GetQangle()
```

```csharp
public float GetQbias()
```

```csharp
public float GetRmeasure()
```

```csharp
public void SetRmeasure(float R_measure)
```
