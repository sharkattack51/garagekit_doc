# TextUtil

テキスト関連のユーティリティ関数を提供します。

```csharp
namespace GarageKit
public class TextUtil
```

#### Static Methods

文字数制限
```csharp
public static string CutoutText(string text, int maxCount)
```

行数を揃える
```csharp
public static string AlignText(string text, int lineCount)
```

改行入りテキストを行文字数及び行数指定で整形
```csharp
public static string CutoutLineAndLfText(string lfText, int maxLineCount, int maxLineStringCount)
```

改行入りテキストを行数指定で整形
```csharp
public static string CutoutLine(string lfText, int maxLineCount)
```

改行を消す
```csharp
public static string RemoveEOL(string text)
```

WWWクラス使用時の半角 `#` のエラーを回避する
```csharp
public static string EscapeSingleByteSharpForWWW(string text)
```

テキストのエンコード変換
```csharp
public static string ConvertEncoding(string srcString, Encoding destEncording)
```

マルチバイト文字でのバイト数を考慮した Substring
```csharp
public static string SubstringDoubleByte(string srcString, int startIndex, int endIndex, Encoding encoding)
```

マルチバイト文字でのバイト数を考慮した文字数カウント
```csharp
public static int MultiByteLength(string srcString, Encoding encoding)
```

マルチバイト文字の確認
```csharp
public static bool IsMultiByteChar(char srcChar, Encoding encoding)
```

TextMesh が指定した幅に収まるかチェックし収まらない場合は改行する
```csharp
public static void CalcTextBox(TextMesh textMesh, float width = 1000.0f)
```

IP アドレスとポート番号に分割しての文字列パース
```csharp
public static bool ParseIpAndPort(string ipStr, out string ip, out int port)
```
