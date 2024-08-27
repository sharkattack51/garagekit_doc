# ContentsDownLoader

Download and save and manage external data.

```csharp
namespace GarageKit
public class ContentsDownLoader : MonoBehaviour
```

#### Inheritance

`ContentsDownLoader` -> `MonoBehaviour`

#### Static Methods

Get the save destination path of downloaded external data
```csharp
public static string ContentsDataPath { get; }
```

#### Methods

Download completion event
```csharp
public event OnLoadCompleteDelegate OnLoadComplete
```

Download error event
```csharp
public event OnLoadErrorDelegate OnLoadError
```

Get the latest download destination path
```csharp
public string LatestContentsPath { get; }
```

Check that the download is in progress
```csharp
public bool IsLoading { get; }
```
