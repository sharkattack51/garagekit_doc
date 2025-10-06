# EnumLabelAttribute

enum 型の各値に `[Label("ラベル名")]` のアトリビュートを付与して、値とは別のラベル文字列を取得できます。

```csharp
namespace GarageKit
public class EnumAttribute
```

#### Methods

ラベル名の取得
```csharp
public static string LabelAttribute(this Enum value)
```

ラベル名配列の取得
```csharp
 public static string[] LabelAttributes<T>() where T : Enum
```

#### Example

```csharp
enum TIER_TYPE
{
    [Label("上")]
    UPPER = 0,

    [Label("中")]
    MIDDLE,

    [Label("下")]
    BOTTOM
}

// enum オブジェクトの値からラベル名を取得する
string label = TIER_TYPE.UPPER.LabelAttribute(); // "上"

// 宣言された enum 型からラベル名配列を取得する
string[] labels = EnumLabelAttribute.LabelAttributes<TIER_TYPE>(); // [ "上", "中", "下" ]
```
