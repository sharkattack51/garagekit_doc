# ButtonObjectEvent

コライダーが設定されているオブジェクトに対して、クリック操作のボタンイベントを設定できるようにします。uGUI は利用しないので、全ての 3D オブジェクトに対して利用可能できます。マウス & タッチ対応。

> [!IMPORTANT]
> TouchScript パッケージを利用の場合はソースコード内の #define 定義を有効にしてください。

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
|inputType|[INPUT_TYPE](#input_type)|入力タイプ|
|buttonType|[BUTTON_TYPE](#button_type)|ボタン実行タイプ|
|asFirstResponder|bool|最前面の場合に実行|
|asToggle|bool|トグルボタン設定|
|PressBtnsTotal|int|押されているボタンの総数|

#### Enums

##### __INPUT_TYPE__

|enums|description|
|:--|:--|
|MOUSE|マウスでの操作|
|TOUCH|タッチでの操作|

##### __BUTTON_TYPE__

|enums|description|
|:--|:--|
|CLICK|クリック時実行|
|PRESS|プレス時実行|
|RELEASE|リリース時実行|
|PRESSHOLD|プレス保持で実行|

#### Static Methods

全 ButtonObjectEvent コンポーネントの入力タイプを変更
```csharp
public static void SetAllInputType(INPUT_TYPE type)
```

#### Methods

ボタン有効確認
```csharp
public bool IsEnableButton { get; }
```

入力有効確認
```csharp
public bool InputEnable { get; }
```

トグルボタン状態確認
```csharp
public bool ToggleState { get; }
```

タッチ入力座標の取得
```csharp
public Vector3 TouchPosition { get; }
```

ボタン実行時コールバック
```csharp
public Action OnButton
```

トグルボタン実行時コールバック
```csharp
public Action<bool> OnToggleButton
```

ボタンプレス時コールバック
```csharp
public Action OnPressButton
```

ボタンリリース時コールバック
```csharp
public Action OnReleaseButton
```

ボタンのホバー状態開始時コールバック
```csharp
public Action OnHoverInButton
```

ボタンのホバー状態終了時コールバック
```csharp
public Action OnHoverExitButton
```

ボタンの状態をリセット
```csharp
public void ResetButton()
```

ボタン有効化
```csharp
public void EnableButton()
```

ボタン無効化
```csharp
public void DisableButton()
```

入力有効化
```csharp
public void EnableInput()
```

入力無効化
```csharp
public void DisableInput()
```

#### Example

- /Scenes/Examples/EventExample.unity
