# ImageLoader

Load images in the specified folder at once.

```csharp
namespace GarageKit
public class ImageLoader : MonoBehaviour
```

#### Inheritance

`ImageLoader` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/imageloader_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|folderPath|string|Folder to load|
|absolute|bool|Absolute path setting|
|autoLoad|bool|Automatic loading start setting|

#### Methods

Loaded image list
```csharp
public Dictionary<string, Texture2D> Images { get; }
```

Loading completion event
```csharp
public event OnLoadCompleteDelegate OnLoadComplete
```

Start loading
```csharp
public void Load(string folderPath)
```
