# RemotePrefs

UDP 通信を利用して PlayerPrefs へのデータ読み書きを行います。

```csharp
namespace GarageKit
[RequireComponent(typeof(UDPReceiver))]
public class RemotePrefs : MonoBehaviour
```

#### Inheritance

`ExternalProcess` -> `MonoBehaviour`

#### Methods

情報更新時直前コールバック
```csharp
public Action<RemotePrefsData> WillUpdatedPrefs
```

情報更新時コールバック
```csharp
public Action<RemotePrefsData> OnUpdatedPrefs
```

#### Example

受信する Json のサンプル
```json
{
    "command": "set", // "set" or "delete" or "delete_all"
    "key": "prefs_key",
    "value_type": "int", // "int" or "float" or "string"
    "int_value": 123
}
```

---

# RemotePrefsData

保存情報の構造体

#### Properties

|member|type|description|
|:--|:--|:--|
|command|string|実行コマンド: "set" or "delete" or "delete_all"|
|key|string|保存情報 キー|
|value_type|string|保存情報 型: "int" or "float" or "string"|
|int_value|int|保存情報 値: int|
|float_value|float|保存情報 値: float|
|string_value|string|保存情報 値: string|
