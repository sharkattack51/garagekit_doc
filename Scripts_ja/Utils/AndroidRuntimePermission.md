# AndroidRuntimePermission

Android 実行時のランタイムパーミッション要求手続きを自動化します。また、関連するユーティリティ関数を提供します。

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
|permissions|string[]|Android パーミッション文字列リスト|

#### Methods

成功時コールバック
```csharp
public Action OnVerifiedPermission
```

失敗時コールバック
```csharp
public Action OnFailurePermission
```

#### Static Methods

現在のアクティビティの取得
```csharp
public static AndroidJavaObject GetActivity()
```

OS バージョンが Android M(Android 6.0 APIレベル23) 以降の確認
```csharp
public static bool IsAndroidMOrGreater()
```

パーミッション保持の確認
```csharp
public static bool HasPermission(string permission)
```

以前にパーミッションを許可しなかった場合に「今後表示しない」を選んでいないか（ダイアログを表示するか）
```csharp
public static bool ShouldShowRequestPermissionRationale(string permission)
```

パーミッション許可のリクエストでダイアログを表示
```csharp
public static void RequestPermission(string[] permissions)
```
