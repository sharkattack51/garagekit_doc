# ObjectUtil

オブジェクト操作関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class ObjectUtil
```

#### Static Methods

子供階層オブジェクトのレイヤーをまとめて設定する
```csharp
public static void SetLayerChildren(GameObject rootObject, int layer, bool changeParent = false)
```

階層全体のバウンディングボックスを取得
```csharp
public static Bounds GetRenderBoundsChildren(GameObject root)
```
