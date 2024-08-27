# TextUtil

Provides text related utility functions.

```csharp
namespace GarageKit
public class TextUtil
```

#### Static Methods

Character limit
```csharp
public static string CutoutText(string text, int maxCount)
```

Align the number of lines
```csharp
public static string AlignText(string text, int lineCount)
```

Format text with line breaks by specifying the number of line characters and number of lines
```csharp
public static string CutoutLineAndLfText(string lfText, int maxLineCount, int maxLineStringCount)
```

Format text with line breaks by specifying the number of lines
```csharp
public static string CutoutLine(string lfText, int maxLineCount)
```

Remove line breaks
```csharp
public static string RemoveEOL(string text)
```

Avoid half-width `#` error when using WWW class
```csharp
public static string EscapeSingleByteSharpForWWW(string text)
```

Text encoding conversion
```csharp
public static string ConvertEncoding(string srcString, Encoding destEncording)
```

Substring considering the number of bytes in multibyte characters
```csharp
public static string SubstringDoubleByte(string srcString, int startIndex, int endIndex, Encoding encoding)
```

Character count considering the number of bytes in multibyte characters
```csharp
public static int MultiByteLength(string srcString, Encoding encoding)
```

Check for multibyte characters
```csharp
public static bool IsMultiByteChar(char srcChar, Encoding encoding)
```

Checks if the TextMesh fits within the specified width, and if it does not fit, breaks a line.
```csharp
public static void CalcTextBox(TextMesh textMesh, float width = 1000.0f)
```

Parse string by splitting it into IP address and port number
```csharp
public static bool ParseIpAndPort(string ipStr, out string ip, out int port)
```
