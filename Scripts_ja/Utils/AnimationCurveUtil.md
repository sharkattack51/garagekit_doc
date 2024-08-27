# AnimationCurveUtil

アニメーションカーブ設定関連のユーティリティ関数を提供します。

reference: UnityEditor.CurveUtility.cs (c) Unity Technologies

```csharp
namespace GarageKit
public class AnimationCurveUtil
```

#### Static Methods

アニメーションカーブの補完をリニアに設定する
```csharp
public static void UpdateAllLinearTangents(AnimationCurve curve)
```

アニメーションカーブ指定キーフレームのタンジェントモード更新
```csharp
public static void UpdateTangentsFromMode(AnimationCurve curve, int index)
```

キーフレームの新規生成と取得
```csharp
public static Keyframe GetNewKey(float time, float value, TangentMode leftAndRight)
public static Keyframe GetNewKey(float time, float value, TangentMode left, TangentMode right)
```

キーフレームのタンジェントモード取得
```csharp
public static TangentMode GetKeyTangentMode(int tangentMode, int leftRight)
public static TangentMode GetKeyTangentMode(Keyframe keyframe, int leftRight)
```

キーフレームの左右ハンドル連結を外す
```csharp
public static void SetKeyBroken(object keyframe, bool broken)
```

#### Enums

##### __TangentMode__

|enums|description|
|:--|:--|
|Editable|エディット|
|Smooth|スムーズ|
|Linear|リニア|
|Stepped|ステップ|
