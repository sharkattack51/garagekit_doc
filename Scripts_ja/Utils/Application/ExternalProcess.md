# ExternalProcess

外部プロセスを起動します。

```csharp
namespace GarageKit
public class ExternalProcess : MonoBehaviour
```

#### Inheritance

`ExternalProcess` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/externalprocess_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|exePath|string|実行ファイルのパス|
|pathFromStreamingAssets|bool|StreamingAssets からの読み込みフラグ|
|arguments|string|実行時パラメータ引数|
|startupOnStart|bool|`Start()` での自動実行フラグ|
|showWindow|bool|プロセス実行時のウィンドウ表示|

#### Methods

内部プロセス ID の取得
```csharp
public int ProcId { get; }
```

プロセスの実行状態
```csharp
public bool IsRunning { get; }
```

プロセスを開始
```csharp
public void StartProcess()
```
