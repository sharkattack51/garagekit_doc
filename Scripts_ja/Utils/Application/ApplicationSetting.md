# ApplicationSetting

外部設定ファイル ApplicationSetting.xml を読み込んでアプリケーションに反映できます。xml は MonoBehaviour の `Awake()` で読み込まれるため、`Start()` 以降のタイミングで利用することができます。

```csharp
namespace GarageKit
public class ApplicationSetting : MonoBehaviour
```

#### Inheritance

`ApplicationSetting` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/applicationsetting_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|loadFrom|[XML_FROM](#xml_from)|xml ファイルの読み込み先|
|xmlFile|string|xml ファイル名|

#### Enums

##### __XML_FROM__

|enums|description|
|:--|:--|
|STREAMING_ASSETS|StreasmingAssets フォルダ|
|PROJECT_DIRECTORY|プロジェクトフォルダ|
|CURRENT_WORK_DIRECTORY|カレントフォルダ|

#### Static Methods

シングルトンインスタンスの取得
```csharp
public static ApplicationSetting Instance { get; }
```

#### Methods

xml 生データテーブル
```csharp
public Dictionary<string, string> RawData { get; }
```

データ有効確認
```csharp
public bool IsValid { get; }
```

xml 読み込み完了コールバック
```csharp
public Action OnLoadXML
```

xml 読み込み
```csharp
public void LoadXML()
```

xml 項目名から string 値の取得
```csharp
public string GetString(string key, string defaultValue = "")
```

xml 項目名から bool 値の取得
```csharp
public bool GetBool(string key, bool defaultValue = false)
```

xml 項目名から int 値の取得
```csharp
public int GetInt(string key, int defaultValue = 0)
```

xml 項目名から float 値の取得
```csharp
public float GetFloat(string key, float defaultValue = 0.0f)
```

xml 項目名から string 配列の取得
```csharp
public string[] GetStringArray(string key, string separator = ",")
```

xml 項目名から int 配列の取得
```csharp
public int[] GetIntArray(string key, string separator = ",", int defaultValue = 0)
```

xml 項目名から float 配列の取得
```csharp
public float[] GetFloatArray(string key, string separator = ",", float defaultValue = 0.0f)
```

xml 項目名から bool 配列の取得
```csharp
public bool[] GetBoolArray(string key, string separator = ",", bool defaultValue = false)
```

xml 項目名からフォーマット定義された DateTime 値の取得
```csharp
public DateTime GetFormattedDateTime(string key, string format = "HH:mm:ss")
```

xml 項目名から DateTime 値の取得
```csharp
public DateTime GetDateTime(string key)
```

xml 項目名から Vector3 値の取得
```csharp
public Vector3 GetVector3(string key, string separator = ",", Vector3 defaultValue = default(Vector3))
```

xml 項目名から Vector2 値の取得
```csharp
public Vector2 GetVector2(string key, string separator = ",", Vector2 defaultValue = default(Vector2))
```

xml 項目名から RGB 0.0-1.0 として Color 値の取得
```csharp
public Color GetColor(string key, string separator = ",", Color defaultValue = default(Color))
```

xml 項目名から RGB 0-255 として Color 値の取得
```csharp
public Color GetColor255(string key, string separator = ",", Color defaultValue = default(Color))
```

#### Example

- /Scenes/Examples/ApplicationSettingExample.unity

```csharp
bool isDebug = ApplicationSetting.Instance.GetBool("IsDebug");
int gameTime = ApplicationSetting.Instance.GetInt("GameTime");
string text = ApplicationSetting.Instance.GetString("Text");
```

- StreamingAssets/ApplicationSetting.xml

```xml
<?xml version="1.0" encoding="utf-8"?>
<data>
    <item name="IsDebug" value="true"/>
    <item name="GameTime" value="10"/>
    <item name="Text" value="this is test."/>
</data>
```
