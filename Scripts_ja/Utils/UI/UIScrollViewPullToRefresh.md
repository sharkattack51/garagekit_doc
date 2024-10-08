# UIScrollViewPullToRefresh

スクロールビューを下に引いて内容を更新する機能のコンポーネント

```csharp
namespace GarageKit
public class UIScrollViewPullToRefresh : MonoBehaviour
```

#### Inheritance

`UIScrollViewPullToRefresh` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/uiscrollviewpulltorefresh_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|uiScrlRect|ScrollRect|操作対象のScrollRectの参照|
|indicatorImg|Image|インジケータイメージの参照|

#### Methods

下に引く操作開始のコールバック
```csharp
public Action OnPullStart
```

下に引く操作キャンセルのコールバック
```csharp
public Action OnPullCancel
```

下に引く操作でスクロール閾値を越えた時のコールバック
```csharp
public Action OnPullOverTh
```

下に引く操作を終了してリフレッシュ処理時のコールバック
```csharp
public Action OnPullToRefresh
```
