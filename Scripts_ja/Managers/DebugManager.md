# DebugManager

デバッグ用の機能を管理します。全てのデバッグ用機能は isDebug フラグによって管理されるようにすると便利です。

```csharp
namespace GarageKit
[RequireComponent(typeof(VisibleMouseCursor))]
public class DebugManager : ManagerBase
```

#### Inheritance

`DebugManager` -> [ManagerBase](~/Scripts_ja/Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/debugmanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|isDebug|bool|デバッグ状態管理用フラグ|
|useIngameDebugConsole|bool|[IngameDebugConsole](https://openupm.com/packages/com.yasirkula.ingamedebugconsole/) パッケージ利用の有無|
|useGraphy|bool|[Graphy](https://openupm.com/packages/com.tayx.graphy/) パッケージ利用の有無|

#### Example

```csharp
// デバッグ状態の確認
if(AppMain.Instance.debugManager.isDebug)
    Debug.Log("debug is true");
```
