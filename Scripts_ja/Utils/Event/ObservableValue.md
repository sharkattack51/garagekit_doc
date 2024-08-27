# ObservableValue

値を監視して更新変化があった場合にコールバックを実行します。

```csharp
namespace GarageKit
public class ObservableValue<T>
```

#### Inheritance

`ObservableValue<T>`

#### Methods

値の取得更新
```csharp
public T Value { get; set; }
```

値に更新変化があった場合にコールバック
```csharp
public Action<T> OnValueChange
```
