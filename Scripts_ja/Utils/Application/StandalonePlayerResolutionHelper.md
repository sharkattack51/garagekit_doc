# StandalonePlayerResolutionHelper

Windows の StandalonePlayer 実行時に、レジストリに自動保存される解像度設定を削除して、次回起動時に間違った解像度で実行される問題を回避します。

> [!IMPORTANT]
> Windows 以外では利用しません。

> [!IMPORTANT]
> 利用する場合は PlayerSettings の ApiCompatibilityLevel を `.NET Framework` に変更します。

```csharp
namespace GarageKit
[ExecuteInEditMode]
public class StandalonePlayerResolutionHelper : MonoBehaviour
```

#### Inheritance

`StandalonePlayerResolutionHelper` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/standaloneplayerresolutionhelper_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|playerSettingsCompanyName|string|プレイヤー設定の CompanyName|
|playerSettingsProductName|string|プレイヤー設定の ProductName|

> [!IMPORTANT]
> OnApplicationQuit() で実行されるため、プロセス Kill や Shutdown コマンドなど、正常終了以外ではレジストリから削除されません。

