# ARKitCoachingOverlay

iOS ARKit のネイティブ機能のコーチングビューをコントロールします。
https://developer.apple.com/documentation/arkit/arcoachingoverlayview

> [!IMPORTANT]
> 利用の際はソースコード内の #define 定義を有効にしてください。

```csharp
namespace GarageKit.ARFoundationExtention
[RequireComponent(typeof(ARSession))]
public class ARKitCoachingOverlay : MonoBehaviour
```

#### Inheritance

`ARKitCoachingOverlay` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/arkitcoachingoverlay_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|Goal|CoachingGoal|追跡要件を指示する為のゴール|
|ActivatesAutomatically|bool|自動有効化|

#### Enums

##### __CoachingGoal__

|enums|description|
|:--|:--|
|Tracking|ワールドトラッキング|
|HorizontalPlane|水平面|
|VerticalPlane|垂直面|
|AnyPlane|任意の平面|

#### Methods

コーチング機能のサポート確認
```csharp
public bool supported { get; }
```

コーチングの有効化
```csharp
public void ActivateCoaching(bool animated)
```

コーチングの無効化
```csharp
public void DisableCoaching(bool animated) 
```
