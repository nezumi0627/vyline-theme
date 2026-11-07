# vyline-theme

Vyline のテーマ（VyTheme）プリセット集です。

`@vyline/themes` パッケージとして `THEME_PRESETS` と `VyTheme` 型を提供し、Vyline 本体はこれを読み込むだけ。テーマの追加・変更はこのリポジトリで行います。

## テーマの追加

1. `src/index.ts` の `THEME_PRESETS` にエントリを追加
2. 必須トークン: `id`, `name`, `accent`, `accentContrast`, `bg`, `surface`, `surface2`, `sidebar`, `text`, `textDim`, `border`, `msgIn`, `msgOut`, `msgInText`, `msgOutText`, `radius`, `chatBg`, `pattern`

### 実験的な表示トークン

`VyTheme` は任意の背景画像項目 `chatImage` と、背景画像だけに適用する `chatBackgroundBlur`（`0`〜`24` px）を提供します。背景画像・ぼかし機能はホストアプリが Beta 同意で明示的に有効化した場合だけ適用してください。`chatBackgroundBlur` を省略した場合は `6px` を初期値として使用できます。メッセージや入力欄などの前景レイヤーにはぼかしを適用しません。

## ライセンス

MIT
