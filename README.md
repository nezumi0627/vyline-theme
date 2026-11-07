# vyline-theme

Vyline のテーマ（VyTheme）プリセット集です。

`@vyline/themes` パッケージとして `THEME_PRESETS` と `VyTheme` 型を提供し、Vyline 本体はこれを読み込むだけ。テーマの追加・変更はこのリポジトリで行います。

## テーマの追加

1. `src/index.ts` の `THEME_PRESETS` にエントリを追加
2. 必須トークン: `id`, `name`, `accent`, `accentContrast`, `bg`, `surface`, `surface2`, `sidebar`, `text`, `textDim`, `border`, `msgIn`, `msgOut`, `msgInText`, `msgOutText`, `radius`, `chatBg`, `pattern`

### 実験的な表示トークン

`VyTheme` は任意項目として `acrylic`, `acrylicOpacity`, `acrylicBlur` を提供します。これらはホストアプリが Beta 同意で明示的に有効化した場合だけ適用してください。省略時はアクリル表示を無効として扱い、値はそれぞれ不透明度 `0.82`、ぼかし `16px` を初期値にできます。背景画像は従来の任意項目 `chatImage` を使います。

## ライセンス

MIT
