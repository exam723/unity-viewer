# Unity アセットバンドル ビューア

端末内だけで UnityFS アセットバンドルを解析し、**画像（Texture2D / Sprite）・音声（AudioClip）・動画（VideoClip）** を表示・再生・保存できるスマホ向け PWA です。

## 公開 URL

https://exam723.github.io/unity-viewer/

## 使い方

1. 上の URL をスマホのブラウザで開く
2. アセットバンドルファイル、フォルダ内の複数ファイル、または ZIP を選ぶ
3. 一覧からタップしてプレビュー。画像は PNG、音声は WAV、動画は元データで保存（まとめて ZIP も可）

処理はすべて端末内で行われます。ファイルはサーバーに送信されません。

## 対応内容

- **画像**: RGBA32 / ETC2 / ASTC / DXT など（端末デコード）
- **音声**: FSB5 の PCM・IMA ADPCM・FADPCM・GCADPCM・Vorbis（Vorbis は Ogg 再構築後、WAV にデコードして再生。iOS Safari でも再生可能）
- **動画**: VideoClip の MP4 / M4V / MOV / WebM など（ブラウザが再生できる形式はそのまま再生。非対応形式は日本語メッセージ付きでダウンロード可）

## ホーム画面への追加

- iPhone: Safari の共有 →「ホーム画面に追加」
- Android: メニュー →「アプリをインストール」 /「ホーム画面に追加」
