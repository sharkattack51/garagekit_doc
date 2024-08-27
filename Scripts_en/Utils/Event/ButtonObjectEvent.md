# ButtonObjectEvent

Enables you to set a click button event for objects that have a collider set. Since uGUI is not used, it can be used for all 3D objects. Mouse & touch compatible.

> [!IMPORTANT]
> If you are using the TouchScript package, please enable the #define definition in the source code.

```csharp
namespace GarageKit
public class ButtonObjectEvent : MonoBehaviour
```

#### Inheritance

`ButtonObjectEvent` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/buttonobjectevent_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|inputType|[INPUT_TYPE](#input_type)|Input type|
|buttonType|[BUTTON_TYPE](#button_type)|Button execution type|
|asFirstResponder|bool|Execute when in front|
|asToggle|bool|Toggle button settings|
|PressBtnsTotal|int|Total number of buttons pressed|

#### Enums

##### __INPUT_TYPE__

|enums|description|
|:--|:--|
|MOUSE|Mouse operation|
|TOUCH|Touch operation|

##### __BUTTON_TYPE__

|enums|description|
|:--|:--|
|CLICK|Execute on click|
|PRESS|Execute on press|
|RELEASE|Execute on release|
|PRESSHOLD|Execute on press hold|

#### Static Methods

Change input type of all ButtonObjectEvent components
```csharp
public static void SetAllInputType(INPUT_TYPE type)
```

#### Methods

Check button validity
```csharp
public bool IsEnableButton { get; }
```

Check input validity
```csharp
public bool InputEnable { get; }
```

Check toggle status
```csharp
public bool ToggleState { get; }
```

Get touch input coordinates
```csharp
public Vector3 TouchPosition { get; }
```

Button execution callback
```csharp
public Action OnButton
```

Toggle button execution callback
```csharp
public Action<bool> OnToggleButton
```

Button press execution callback
```csharp
public Action OnPressButton
```

Button release execution callback
```csharp
public Action OnReleaseButton
```

Button hover start callback
```csharp
public Action OnHoverInButton
```

Button hover end callback
```csharp
public Action OnHoverExitButton
```

Reset button status
```csharp
public void ResetButton()
```

Enabling button
```csharp
public void EnableButton()
```

Disabling button
```csharp
public void DisableButton()
```

Enabling input
```csharp
public void EnableInput()
```

Disabling input
```csharp
public void DisableInput()
```

#### Example

- /Scenes/Examples/EventExample.unity
