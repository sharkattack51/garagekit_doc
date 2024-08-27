# ICsvWritable

CSV 書き込みに対応するためのデータクラスインターフェース

```csharp
namespace GarageKit.CSV
public interface ICsvWritable
```

#### Methods

ヘッダー行文字列の取得
```csharp
string GetCsvHeader()
```

行文字列の取得
```csharp
string ToCsvRowString()
```
