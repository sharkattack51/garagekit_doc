# AnimationByStep

Animation コンポーネントのステップ実行をします。

```csharp
namespace GarageKit
public class AnimationByStep : MonoBehaviour
```

#### Inheritance

`AnimationByStep` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/animationbystep_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|anim|Animation|Animation の参照|
|speed|float|ステップ再生スピード|
|useSmooth|bool|スムーズ更新|

#### Methods

アニメーションのステップ実行
```csharp
public void Step()
```

アニメーションのリセット
```csharp
public void Reset()
```

アニメーション位置の指定
```csharp
public void SetSeconds(float sec)
```

現在のアニメーション位置を取得
```csharp
public float GetSeconds()
```

現在のアニメーション尺を取得
```csharp
public float GetDuration()
```
