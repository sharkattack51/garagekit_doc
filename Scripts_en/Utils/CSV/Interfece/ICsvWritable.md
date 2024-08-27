# ICsvWritable

Data class interface to support CSV writing

```csharp
namespace GarageKit.CSV
public interface ICsvWritable
```

#### Methods

Get header row string
```csharp
string GetCsvHeader()
```

Get line string
```csharp
string ToCsvRowString()
```
