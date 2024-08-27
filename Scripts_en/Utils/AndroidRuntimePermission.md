# AndroidRuntimePermission

Automates the runtime permission request procedure when running Android. It also provides related utility functions.

```csharp
namespace GarageKit
public class AndroidRuntimePermission : ManagerBase
```

#### Inheritance

`AndroidRuntimePermission` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/androidruntimepermission_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|permissions|string[]|Android permission string list|

#### Methods

Callback on success
```csharp
public Action OnVerifiedPermission
```

Callback on failure
```csharp
public Action OnFailurePermission
```

#### Static Methods

Get current activity
```csharp
public static AndroidJavaObject GetActivity()
```


Check that the OS version is Android M (Android 6.0 API level 23) or later
```csharp
public static bool IsAndroidMOrGreater()
```

Check have permissions
```csharp
public static bool HasPermission(string permission)
```

If you previously denied permission, have you selected "Don't show this again" (should a dialog be displayed)?
```csharp
public static bool ShouldShowRequestPermissionRationale(string permission)
```

Show dialog when requesting permission
```csharp
public static void RequestPermission(string[] permissions)
```
