# ARTrackedImageMarkerManager

AR イメージマーカーのトラッキング機能を管理します。マーカー認識開始時のオブジェクト生成機能や、認識開始時と認識終了時のイベントを利用できます。

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit.ARFoundationExtention
[DisallowMultipleComponent]
[RequireComponent(typeof(ARTrackedImageManager))]
public class ARTrackedImageMarkerManager : MonoBehaviour
```

#### Inheritance

`ARTrackedImageMarkerManager` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/artrackedimagemarkermanager_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|trackedImageMarkerDatas|List<[ARTrackedImageMarkerData](#artrackedimagemarkerdata)>|生成するイメージマーカー プレハブデータリスト|
|destroyOnInvisible|bool|画面外判定で自動 Destroy を行う|
|numberOfTrackingImage|int|同時トラッキング可能な最大イメージ数|

#### Methods

トラッキング中のイメージテーブル
```csharp
public Dictionary<string, ARTrackedImage> TrackedImages { get; }
```

イメージマーカー認識開始時コールバック
```csharp
public Action<ARTrackedImage> OnAddedImageMarker
```

イメージマーカー認識終了時コールバック
```csharp
public Action<ARTrackedImage> OnRemoveImageMarker
```

トラッキング中マーカーからイメージマーカー名での削除
```csharp
public void RemoveImageMarkerByImageName(string imageName)
```

全トラッキング中マーカーのリセット
```csharp
public void ResetImageMarkers()
```

---

# ARTrackedImageMarkerData

イメージマーカーに対応する生成プレハブデータの構造体

```csharp
namespace GarageKit.ARFoundationExtention
[Serializable]
public class ARTrackedImageMarkerData
```

#### Properties

|member|type|description|
|:--|:--|:--|
|imageName|string|イメージマーカー名|
|imageMarkerPrefab|GameObject|生成するプレハブの参照|
