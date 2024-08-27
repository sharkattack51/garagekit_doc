# OnCollisionHandler

Execute MonoBehaviour's OnCollision and OnTrigger functions in a callback.

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
