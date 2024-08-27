# CsvReader

CSV ファイルの読み込み用クラス

```csharp
namespace GarageKit.CSV
public class CsvReader
```

#### Inheritance

`CsvReader`

#### Static Methods

2 次元配列のデバッグ用出力
```csharp
static public void DebugLogGrid(string[,] grid)
```

#### Methods

データ読み込み確認
```csharp
public bool IsVaild { get； }
```

2 次元配列の取得
```csharp
public string[,] CsvGrid { get; }
```

CSV ファイルの読み込み
```csharp
public void Read(string file)
```
