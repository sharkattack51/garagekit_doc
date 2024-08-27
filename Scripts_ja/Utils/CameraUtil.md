# CameraUtil

カメラ関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class CameraUtil
```

#### Static Methods

レイヤーからカメラを取得
```csharp
public static Camera FindCameraForLayer(int layer)
```

デプスによる全カメラリストを取得
```csharp
public static List<Camera> GetCameraListByDepth()
```

スクリーン座標をカメラ座標で正規化(-1.0～1.0)
```csharp
public static Vector3 NormalizeScreenPosition(Camera orthoCamera, Vector3 screenPosition)
```

Viewport で画面をはみ出した場合の座標を修正する
```csharp
public static Vector3 ViewportProtrusion(Vector3 viewportPosition, Vector2 ratio)
```