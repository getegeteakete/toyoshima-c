# とよしま矯正歯科 AI統合管理ダッシュボード

## Vercelへのデプロイ手順

### 方法1: Vercel CLI（推奨）
```bash
npm i -g vercel
cd dashboard
vercel --prod
```
→ 表示されたURLがダッシュボードのアドレスになります

### 方法2: GitHub経由
1. このフォルダをGitHubリポジトリにプッシュ
2. vercel.com でリポジトリをインポート
3. 自動デプロイ完了

### 方法3: Vercelドラッグ&ドロップ
1. vercel.com/new を開く
2. dashboardフォルダをドラッグ&ドロップ
3. 完了

## 接続設定
デプロイ後、「API設定」画面から:
- **Supabase**: Project URL + Anon Key を入力 → 接続テスト
- **WordPress**: サイトURL（読み取りは自動）
- **Claude API**: claude.ai上では自動接続

## Supabaseテーブル名の確認
Supabase管理画面 → Table Editor で
予約データが入っているテーブル名を確認し
「予約テーブル名」に入力してください。
(例: appointments, bookings, reservations など)
