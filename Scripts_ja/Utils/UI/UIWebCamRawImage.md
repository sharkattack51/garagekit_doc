# UIWebCamRawImage

Web カメラを利用する uGUI RawImage 設定を簡易化します。

```csharp
namespace GarageKit
[RequireComponent(typeof(RawImage))]
public class UIWebCamRawImage : MonoBehaviour
```

#### Inheritance

`UIWebCamRawImage` -> `MonoBehaviour`

#### Inspector

<img src="~/image/script_reference/webcamrawimage_inspector.png" width="500px"/>

#### Properties

|member|type|description|
|:--|:--|:--|
|webcamPlayOnStart|bool|Start() での再生開始|
|deviceName|string|カメラデバイス名の指定|
|deviceIndex|int|カメラデバイス ID の指定|
|requestedWidth|int|カメラ映像 幅の指定|
|requestedHeight|int|カメラ映像 高さの指定|
|requestedFPS|int|カメラ映像 FPS の指定|
|anisoLevel|int|映像テクスチャの異方性フィルタリングレベル|
|filteMode|FilterMode|映像テクスチャのフィルターモード|
|wrapMode|TextureWrapMode|映像テクスチャの繰り返しモード|
|isAutoScreenAspect|bool|アスペクトの自動設定|
|isMirror|bool|左右反転設定|
|appOrientation|[APP_ORIENTATION](#app_orientation)|画面の向き|

#### Enums

##### __APP_ORIENTATION__

|enums|description|
|:--|:--|
|PORTRAIT|ポートレイト / 端末縦位置|
|LANDSCAPE|ランドスケープ / 端末横位置|

#### Methods

WebCamTexture の取得
```csharp
public WebCamTexture WebCamTexture { get; }
```

Web カメラの開始
```csharp
public IEnumerator WebcamPlay()
```

Web カメラの停止
```csharp
public void WebcamStop()
```

Web カメラが開かれているかの確認
```csharp
public bool IsWebcamPlay()
```
