# ARSessionStartHelper

ARSession コンポーネントのヘルパークラスです。端末内の AR システムのインストール確認と AR セッション開始を自動管理します。

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit.ARFoundationExtention
[RequireComponent(typeof(ARSession))]
public class ARSessionStartHelper : MonoBehaviour
```

#### Inheritance

`ARSessionStartHelper` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arsessionstarthelper_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|arSession|ARSession|ARSession の参照|

#### Methods

AR 機能の初期化失敗時コールバック
```csharp
public Action OnFailARSession
```

AR ライブラリのインストールリクエスト時コールバック(ARCore)
```csharp
public Action OnRequestARLibInstall
```

AR 機能の初期化完了コールバック
```csharp
public Action OnReadyAR
```
