# foRPro マイページ - デザインプレビュー

このリポジトリは、HubSpotで開発しているfoRProマイページのメンバーシップ機能の**デザインプレビュー版**です。

## ⚠️ 重要な注意事項

- **これは静的HTMLプレビューです**
- 実際のログイン・登録機能は動作しません
- デザインとUIの確認を目的としています
- 実際の機能はHubSpot CMS上で動作します

## 📄 ページ一覧

- `login.html` - サインインページ
- `register.html` - アカウント登録ページ
- `reset-password.html` - パスワードリセットページ
- `logout.html` - ログアウトページ

## 🎨 デザインシステム

### カラー
- プライマリ: `#8B7355` (ブラウン)
- プライマリ(ホバー): `#6D5A45` (ダークブラウン)
- 背景: `#fafafa` (ライトグレー)
- ボーダー: `#e8e8e8`

### フォント
- システムフォント: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto`
- 基本サイズ: `14px`
- 見出し: `18px` (font-weight: 600)

## 🚀 ローカルで確認する方法

### 方法1: ブラウザで直接開く
1. `login.html` をダブルクリック
2. ブラウザで表示されます

### 方法2: ローカルサーバーを起動
```bash
# Python 3がインストールされている場合
cd HubSpotpreview
python -m http.server 8000

# ブラウザで http://localhost:8000/login.html にアクセス
```

## 📦 ファイル構成

```
HubSpotpreview/
├── login.html              # ログインページ
├── register.html           # 登録ページ
├── reset-password.html     # パスワードリセット
├── logout.html            # ログアウト
├── css/
│   └── mypage-common.css  # 共通スタイル
├── images/                # 画像フォルダ(予定)
└── README.md              # このファイル
```

## 🔐 セキュリティについて

このプレビュー版には以下が含まれていません：
- HubSpotアカウントID
- APIキー
- 内部URL
- 個人情報

安心してチームで共有できます。

## 💡 実装について

実際のHubSpot本番環境では：
- HubLテンプレート言語を使用
- `{% member_login %}` などのHubSpot専用モジュールを使用
- `request.contact` でログインユーザー情報を取得
- アクセスグループによる制御

が実装されています。

## 🤝 フィードバック

デザインについてのフィードバックをお待ちしております！

---

**開発者**: Claude AI + TaichiShibuki
**作成日**: 2025年10月29日
