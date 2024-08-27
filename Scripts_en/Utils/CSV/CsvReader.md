# CsvReader

Class for reading CSV files

```csharp
namespace GarageKit.CSV
public class CsvReader
```

#### Inheritance

`CsvReader`

#### Static Methods

Debugging output for two dimensional arrays
```csharp
static public void DebugLogGrid(string[,] grid)
```

#### Methods

Check data validity
```csharp
public bool IsVaild { get； }
```

Get two dimensional array
```csharp
public string[,] CsvGrid { get; }
```

Read CSV file
```csharp
public void Read(string file)
```
