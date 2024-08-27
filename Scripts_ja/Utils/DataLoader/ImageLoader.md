# ImageLoader

指定したフォルダ内の画像を一括読み込みします。

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
|folderPath|string|読み込み対象のフォルダ|
|absolute|bool|絶対パス設定|
|autoLoad|bool|自動読み込み開始設定|

#### Methods

読み込み済み画像リスト
```csharp
public Dictionary<string, Texture2D> Images { get; }
```

読み込み完了イベント
```csharp
public event OnLoadCompleteDelegate OnLoadComplete
```

読み込み開始
```csharp
public void Load(string folderPath)
```
