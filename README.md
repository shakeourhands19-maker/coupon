# Coupon Box

レシートなどに付属するクーポンを、写真と情報のセットでスマートフォン本体に保存するPWAです。

## GitHub Pages 公開
Settings → Pages → Build and deployment で **Deploy from a branch** を選択し、Branch を **main / (root)** に設定してください。

公開URL: https://shakeourhands19-maker.github.io/coupon/

## 機能
- カメラ撮影・画像選択
- Tesseract.jsによる日本語・英語OCR
- OCR結果の編集（店舗名・割引内容・期限・条件）
- IndexedDBへの写真・情報の端末内保存
- 未使用／使用済み／期限切れ管理
- JSONバックアップと復元（バックアップボタン長押し／PCでは右クリック）

## 保存とプライバシー
クーポン写真と登録情報はIndexedDBに保存し、アプリのサーバーへアップロードしません。OCRエンジンと言語データは初回利用時にCDNから取得されます。ブラウザのデータ消去や端末故障でデータが失われる可能性があるため、定期的にバックアップしてください。

## OCRについて
OCRは読み間違えることがあります。特に日付・利用条件は必ず元写真と照合してください。初回のOCRには通信が必要で、言語データのダウンロードに時間がかかる場合があります。
