# UIFadeGroupComponent

CanvasGroup のフェード処理を管理します。

```csharp
namespace GarageKit
public class UIFadeGroupComponent : MonoBehaviour
```

#### Inheritance

`UIFadeGroupComponent` -> `MonoBehaviour`

#### Methods

フェードのリセット
```csharp
public void ResetFade()
```

フェードの開始
```csharp
public void StartFade(float fixTime = 5.0f, float tweenTime = 0.5f)
```

カメラ位置に対して距離による UI 位置をセット
```csharp
public void SetUiPosition3D(Vector3 camPos, Vector3 targetPos, float height = 1.8f, float depth = 1.5f)
```
