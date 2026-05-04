# PixelPerfect Layer

デザインカンプとコーディング結果の画像を比較し、AIがCSSのズレを自動分析・修正案を提示するPWAツールです。

## 特徴

- **Groq Vision API** (llama-4-scout-17b) によるAI画像比較
- デザインカンプ + スクリーンショットの2画像アップロード対応
- HTML/CSSを貼り付けると分析精度UP
- ズレの重要度（HIGH / MED / LOW）で分類
- 修正CSSをワンクリックコピー
- APIキーはlocalStorageに保存（サーバー不要）
- PWA対応（ホーム画面追加可能）

## 使い方

1. ⚙️ 設定からGroq APIキー（`gsk_...`）を入力・保存
2. デザインカンプ画像をアップロード
3. ブラウザのスクリーンショットをアップロード
4. 「AIでズレを分析する」ボタンをクリック
5. 結果の修正CSSをコピーして使用

## 注意事項

- Groq Visionのbase64画像サイズ制限: **4MB以内**
- 大きな画像は事前に縮小してください
- APIキーはブラウザのlocalStorageにのみ保存されます

## デプロイ

Cloudflare Pages Direct Uploadで `index.html` と `manifest.json` をアップロードするだけで使えます。

## Layer シリーズ

- [Lotolayer](https://lotolayer.toshihide3.workers.dev/) - 宝くじ予測
- [Keirin Layer](https://github.com/toshihideterui) - 競輪予測
- PixelPerfect Layer - デザインズレ分析（本リポジトリ）
