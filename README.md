# ジュエリーポータル 提携のご案内（ジュエリー会社さま向け）

株式会社トライスパイド ／ 商談用の1枚ものWebページ（縦スクロール・操作あり）。

## ファイル構成

```
index.html   ページ本体（CSS・JS・アイコンをすべて内包した単一ファイル）
README.md    このファイル
```

外部ファイルへの依存は **Google Fonts のみ**（Zen Old Mincho / Zen Kaku Gothic New / Instrument Sans）。
画像は使っておらず、アイコンはすべてSVGでHTML内に埋め込んでいます。ビルド作業は不要です。

## GitHub Pages で公開する手順

1. GitHubで新しいリポジトリを作成する（例: `jewelry-partner`）
2. 作成直後の画面で **uploading an existing file** を押し、`index.html` と `README.md` をドラッグ＆ドロップ → **Commit changes**
3. リポジトリの **Settings** → 左メニュー **Pages** を開く
4. **Source** を `Deploy from a branch`、**Branch** を `main` ／ `/ (root)` にして **Save**
5. 1〜2分待つと同じ画面にURLが表示される
   `https://<アカウント名>.github.io/<リポジトリ名>/`

### 公開範囲の注意

**Public リポジトリの GitHub Pages は、URLを知っていれば誰でも閲覧できます。**
本ページは未リリースのサービス資料のため、次のいずれかをご検討ください。

- 社外に出しても差し支えない内容か確認したうえで Public にする
- Private リポジトリのまま Pages を使う（GitHub Pro / Team / Enterprise のプランが必要）
- 商談中だけ共有したい場合は、GitHub Pages ではなく Claude の Artifact リンク（共有オフのまま個別共有）を使う

`index.html` には `<meta name="robots" content="noindex, nofollow">` を入れてあり、検索エンジンへの登録は抑止されます（アクセス制限ではありません）。

## 更新のしかた

`index.html` を編集してコミットすれば、数十秒〜1分でPagesに反映されます。
よく触る箇所は次のとおりです。

| 内容 | 探す場所 |
|---|---|
| 配色 | ファイル先頭の `:root{ --bg: ... }` |
| 見出し・本文 | `<section class="sec">` 単位 |
| 4段階フローの文言 | `<script>` 内の `var STEPS = [...]` |
| 来店確認アニメの画面 | `<script>` 内の `var VS = [...]` |
| レシートの2パターン | `<script>` 内の `var CHAINS = [...]` |
| 管理画面のサンプル | `<script>` 内の `HOME` / `RES` / `PRESET` |

## 掲載内容についての注意

- サービスは開発中、サービス名は仮称です
- 金額・料率・特典の額面は記載していません（契約条件・未確定事項のため）
- 管理画面およびスマートフォンの図は画面イメージで、数値はサンプルです
- 図中のアイコンは説明用の汎用ピクトグラムで、各社のロゴマークではありません
- ジュエリー会社さま向けの資料のため、会場へのレベニューシェアに関する記載は一切含めていません
