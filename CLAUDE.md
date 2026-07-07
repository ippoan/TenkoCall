# TenkoCall - 中間点呼アプリ

トラックドライバーの中間点呼を簡易化する Android アプリ。ボタン一つで「位置情報送信 → 電話発信」を実行する。

## 規範

- **電話番号取得不可の端末では使用不可** — 起動時に `READ_PHONE_NUMBERS` 権限で取得できなければ「この端末では使用できません」で終了する
- **バックエンドは alc-app 経由で rust-alc-api を呼ぶ。直接叩かない**

## ビルド

```bash
cd /home/yhonda/android/TenkoCall   # 192.168.11.60
./gradlew assembleDebug
```

詳細 (アーキテクチャ・技術スタック・API・引き継ぎ残作業) は TenkoCall-map skill を参照
