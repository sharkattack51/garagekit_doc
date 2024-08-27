# CsvWriter

CSV ファイルの書き込み用クラス

```csharp
namespace GarageKit.CSV
public class CsvWriter
```

#### Inheritance

`CsvWriter`

#### Methods

CSV 書き込み
```csharp
public string Write(string file, ICsvWritable data)
public string Write(string file, List<ICsvWritable> datas)
```
