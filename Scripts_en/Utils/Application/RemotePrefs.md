# RemotePrefs

Read and write data to PlayerPrefs using UDP communication.

```csharp
namespace GarageKit
[RequireComponent(typeof(UDPReceiver))]
public class RemotePrefs : MonoBehaviour
```

#### Inheritance

`ExternalProcess` -> `MonoBehaviour`

#### Methods

Callback just before information update
```csharp
public Action<RemotePrefsData> WillUpdatedPrefs
```

Callback when updating information
```csharp
public Action<RemotePrefsData> OnUpdatedPrefs
```

#### Example

Sample of received json
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

Storage information structure

#### Properties

|member|type|description|
|:--|:--|:--|
|command|string|Execution command: "set" or "delete" or "delete_all"|
|key|string|Stored key|
|value_type|string|Stored type: "int" or "float" or "string"|
|int_value|int|Stored value: int|
|float_value|float|Stored value: float|
|string_value|string|Stored value: string|
