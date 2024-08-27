# UserInputManager

ユーザー入力機能を管理します。全てのユーザー入力のコードはここに纏めると便利です。

```csharp
namespace GarageKit
public class UserInputManager : ManagerBase
```

#### Inheritance

`UserInputManager` -> [ManagerBase](../Utils/Manager/Base/ManagerBase.md) -> `MonoBehaviour`

#### Example

デフォルト実装済みキー

|操作キー|機能|
|:--|:--|
|Esc|アプリケーションの終了|
|D|デバッグ機能のトグル|
|R|設定ファイル ApplicationSetting.xml の再読み込み|
|Backspace|現在の GameView をキャプチャーしてデスクトップに画像保存|
