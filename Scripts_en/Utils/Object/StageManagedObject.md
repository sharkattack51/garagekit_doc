# StageManagedObject

Manage visibility of objects. [SceneStateManager](~/Scripts_en/Managers//SceneStateManager.md) is useful when you want to show/hide objects in each state all at once during state transition.

```csharp
namespace GarageKit
public class StageManagedObject : MonoBehaviour
```

#### Inheritance

`StageManagedObject` -> `MonoBehaviour`

#### Static Methods

Hide objects of all StageManagedObject components
```csharp
public static void AllOff()
```

Display objects of all StageManagedObject components in a list
```csharp
public static void ListOn(List<StageManagedObject> ons)
public static void ListOn(StageManagedObject[] ons)
```

#### Methods

Display object
```csharp
public void On()
```

Hide object
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
        // Switching display objects during State transition
        StageManagedObject.AllOff();
        foreach(StageManagedObject obj in enables)
            obj.On();
    }
}
```