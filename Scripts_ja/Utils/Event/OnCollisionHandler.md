# OnCollisionHandler

MonoBehaviour の OnCollision 系関数と OnTrigger 系関数をコールバック化して実行します。

```csharp
namespace GarageKit
[RequireComponent(typeof(Collider))]
public class OnCollisionHandler : MonoBehaviour
```

#### Inheritance

`OnCollisionHandler` -> `MonoBehaviour`

#### Methods

```csharp
public Action<Collision> OnCollisionEnterAction
```

```csharp
public Action<Collision> OnCollisionExitAction
```

```csharp
public Action<Collision> OnCollisionStayAction
```

```csharp
public Action<Collision> OnTriggerEnterAction
```

```csharp
public Action<Collision> OnTriggerExitAction
```

```csharp
public Action<Collision> OnTriggerStayAction
```
