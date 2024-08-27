# ObservableValue

Monitor the value and execute a callback if there is an update change.

```csharp
namespace GarageKit
public class ObservableValue<T>
```

#### Inheritance

`ObservableValue<T>`

#### Methods

Get value update
```csharp
public T Value { get; set; }
```

Callback when there is an update change in the value
```csharp
public Action<T> OnValueChange
```
