# StageManagedObject

オブジェクトの表示 / 非表示を管理します。[SceneStateManager](~/Scripts_ja/Managers//SceneStateManager.md) で State 遷移時に各 State でオブジェクトをまとめて表示 / 非表示させる場合に便利です。

```csharp
namespace GarageKit
public class StageManagedObject : MonoBehaviour
```

#### Inheritance

`StageManagedObject` -> `MonoBehaviour`

#### Static Methods

全 StageManagedObject コンポーネントのオブジェクトを非表示
```csharp
public static void AllOff()
```

全 StageManagedObject コンポーネントのオブジェクトをリストで表示
```csharp
public static void ListOn(List<StageManagedObject> ons)
public static void ListOn(StageManagedObject[] ons)
```

#### Methods

オブジェクトを表示
```csharp
public void On()
```

オブジェクトを非表示
```csharp
public void Off()
```

#### Example

```csharp
public class SampleState : StateBase
{
    public StageManagedObject[] enables;

    public override void StateStart(object context)
    {
        // State 遷移時に表示オブジェクトの切り替え
        StageManagedObject.AllOff();
        foreach(StageManagedObject obj in enables)
            obj.On();
    }
}
```