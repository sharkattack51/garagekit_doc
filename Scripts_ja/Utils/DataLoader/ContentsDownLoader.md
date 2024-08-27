# ContentsDownLoader

外部データをダウンロードしてローカル保存する管理機能を提供します。

```csharp
namespace GarageKit
public class ContentsDownLoader : MonoBehaviour
```

#### Inheritance

`ContentsDownLoader` -> `MonoBehaviour`

#### Static Methods

ダウンロードした外部データの保存先を取得
```csharp
public static string ContentsDataPath { get; }
```

#### Methods

ダウンロード完了イベント
```csharp
public event OnLoadCompleteDelegate OnLoadComplete
```

ダウンロードエラーイベント
```csharp
public event OnLoadErrorDelegate OnLoadError
```

最新のローカル保存先パスの取得
```csharp
public string LatestContentsPath { get; }
```

ダウンロード中の確認
```csharp
public bool IsLoading { get; }
```
