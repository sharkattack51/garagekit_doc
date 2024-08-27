# ApplicationSetting

You can load the external settings file ApplicationSetting.xml and reflect it in the application. xml is loaded by MonoBehaviour's `Awake()`, so it can be used after `Start()`.

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
|loadFrom|[XML_FROM](#xml_from)|Where to load the xml file|
|xmlFile|string|xml file name|

#### Enums

##### __XML_FROM__

|enums|description|
|:--|:--|
|STREAMING_ASSETS|from StreasmingAssets folder|
|PROJECT_DIRECTORY|from Project folder|
|CURRENT_WORK_DIRECTORY|from Current folder|

#### Static Methods

Get a singleton instance
```csharp
public static ApplicationSetting Instance { get; }
```

#### Methods

Xml data table
```csharp
public Dictionary<string, string> RawData { get; }
```

Check data validity
```csharp
public bool IsValid { get; }
```

Xml load completion callback
```csharp
public Action OnLoadXML
```

Load xml
```csharp
public void LoadXML()
```

Get string value from xml item name
```csharp
public string GetString(string key, string defaultValue = "")
```

Get bool value from xml item name
```csharp
public bool GetBool(string key, bool defaultValue = false)
```

Get int value from xml item name
```csharp
public int GetInt(string key, int defaultValue = 0)
```

Get float value from xml item name
```csharp
public float GetFloat(string key, float defaultValue = 0.0f)
```

Get string array from xml item name
```csharp
public string[] GetStringArray(string key, string separator = ",")
```

Get int array from xml item name
```csharp
public int[] GetIntArray(string key, string separator = ",", int defaultValue = 0)
```

Get float array from xml item name
```csharp
public float[] GetFloatArray(string key, string separator = ",", float defaultValue = 0.0f)
```

Get bool array from xml item name
```csharp
public bool[] GetBoolArray(string key, string separator = ",", bool defaultValue = false)
```

Get formatted DateTime from xml item name
```csharp
public DateTime GetFormattedDateTime(string key, string format = "HH:mm:ss")
```

Get DateTime value from xml item name
```csharp
public DateTime GetDateTime(string key)
```

Get Vector3 value from xml item name
```csharp
public Vector3 GetVector3(string key, string separator = ",", Vector3 defaultValue = default(Vector3))
```

Get Vector2 value from xml item name
```csharp
public Vector2 GetVector2(string key, string separator = ",", Vector2 defaultValue = default(Vector2))
```

Get Color value as RGB 0.0-1.0 from xml item name
```csharp
public Color GetColor(string key, string separator = ",", Color defaultValue = default(Color))
```

Get Color value as RGB 0-255 from xml item name
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
