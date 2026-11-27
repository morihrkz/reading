# reading リポジトリの作業指示

「作成文書」（ GitHub Pages で公開する静的サイト。副題 A Reading Room ）のリポジトリである。調査・手順書・資料など、 Claude と作った HTML 文書を保管する。構成は、一覧の `portal.html` 1 枚、文書の `*.html` 、公開サイトのトップに置く装飾ページ `index.html` （後述。触れない）、 `README.md` 、 `future-article-themes.md` （次に書く文書の計画）。ビルド工程と外部ライブラリは使わない。 JavaScript は、 `portal.html` の本文検索と画面操作の補助（後述）のほかには、 `ahamo-migration-guide.html` （チェック状態を保存）、 `plateau-ai-workflow-guide.html` （コード欄のコピーボタン）、 `color-palette.html` （色見本のカードの生成と、色コードのコピー）の 3 本だけが使う。ほかの文書には使わない。

## HTML 文書の意匠
HTML 文書の新規作成にも、既存の文書の意匠の修正・検証にも、ローカルスキル `readable-html-style`(`~/.claude/skills/readable-html-style/SKILL.md`)を使う。

- 文書の意匠の正は、スキル（ `readable-html-style` ）である。配色・寸法・マークアップ・出力前チェックは、すべてスキル側に書かれている。この `CLAUDE.md` にコピーしない。
- 一括変換は、意匠だけを変え、文字列を変えていない。そのため、 `check_readable_html.py` に、本文の書き方に由来する NG が残る文書がある（キッカー・副題・リードの欠如 C03 、番号のない見出し C04 ・ C05 、ラベル後のコロン C11 、裸の URL C10 、脚注の番号の飛び C06 ）。頼まれていないのに直さない。直すときは、本文を直す作業として、ユーザーに相談する。
- 文書ごとの固有の部品（ `dl.summary` ・ `.company` ・ `.compare` ・アニメーションなど）は、その文書の `<style>` に、意匠の CSS の後ろへ足してある。新しく書く指定の色は、 `readable-html-style` の変数を使う。旧 contrast の色の名前（ `--navy` など）は、変換した文書の追加 CSS のための別名で、新しい指定には使わない。 C02 の WARN が出るのは、意図したものである。
  - 例外の色が 1 か所ある。 `electric-motor-guide.html` の整流子の図は、図内の文字が「オレンジ」「緑」と色名を言うので、橙（ `#f26b00` ）と緑（ `#1f8a3b` ）を固有 CSS に足した。ほかの図には足さない。
  - `electric-motor-guide.html` は、 CSS だけで動くアニメーション（停止ボタンつき）を持つ。スキルの `assets/readable-anim.css` と同じ方式（停止ボタン）の固有 CSS で、この文書独自の動きも足してある。
- `electric-motor-guide.html` ・ `election-schedule-japan.html` ・ `us-midterm-2026.html` は、本文が図の色を「青」「紺」「 blue 」と呼ぶので、図の中は紺を保つ（変換スクリプトの `--keep-navy` ）。図の外で紺を使う箇所（ `electric-motor-guide.html` の「青＝ S 極」の文字と、 `us-midterm-2026.html` の凡例）は、固有 CSS で紺にしている。
- `contrast-html-style` は、このリポジトリでは使わない。意匠は排他的で、同じ文書に重ねて適用しない。
- `color-palette.html` には、 contrast も `readable-html-style` も適用していない(適用作業の対象から除いた)。この文書の意匠を直すときは、先にユーザーへ方針を確認する。
- `megumino.html` （経路案内）は、意匠スキル（ `readable-html-style` と旧 `contrast-html-style` ）の対象外である。屋外の小さいスマホで読むための独自の意匠で、この文書の `<style>` が正である。意匠スキルの規約に合わせて直さず、その検査を当てて直さない。
  - 色は意味で使い分ける。白地に黒の文字を基本に、紺 `#00205b` が見出し、黄 `#ffd400` が系統番号と地図の番号、赤 `#b3001b` が降車・目的地、青 `#0022a8` がリンク。文字と地のコントラスト比は 7 以上を保つ。
  - 地図（ `route_1_web.png` 〜 `route_4_web.png` ）は、 OpenStreetMap のデータから描いた横 1080px の PNG である。図の中と説明文の両方に、出典（ © OpenStreetMap contributors ）を入れる。地図の番号は、図の下の `ol.steps` の番号と一致させる。描画スクリプトは残していない。
- スキルの対象は文書だけで、 `portal.html` は含まない。 `portal.html` は一覧ページで、仕様は後述の「 portal.html の構造」にある。 portal 専用の意匠なので、意匠スキルの検査（ `check_readable_html.py` ・ `check_contrast_html.py` ）は当てない。
- 文書の冒頭部（ `.kicker` ・ `.subtitle` ・ `.lede` ・ `.meta` ）の有無は、文書ごとに揺れている。揃っていない文書を見つけても、頼まれていないのに揃えない。新しい文書は、スキルの定めに従う。

## portal.html の掲載対象外（ 3 件）
次の 3 件は、今も将来も `portal.html` に載せない。カードも、新着も、件数にも入れない。掲載を提案しない。

- `index.html`
- `megumino.html`
- `color-palette.html`

## index.html には触れない
`index.html` は、公開サイトのトップ（ `https://morihrkz.github.io/reading/` ）に表示される装飾ページである。ダーク配色の背景で CSS アニメーションが動く、英語の 1 枚物で、文書の一覧ではない。 `portal.html` へのリンクも持たない。この構成は意図的なものである。

- **編集しない。** 頼まれても、まず意図の確認を取る。
- 整合の見直し、件数の更新、意匠の統一、検査（ `font-family` の検出など）、未使用 CSS の整理のどれにも含めない。
- 文書の本数を数えるときは、 `index.html` と `portal.html` を除く。
- 唯一のダーク配色（ `color-scheme: dark` ）なので、後述のダークモードの検証でも、対象から外す。

## 規約の書き方
- 規約の本体は、文書ならスキル（ `SKILL.md` ）、 `portal.html` ならこの `CLAUDE.md` に置く。どちらも、既存ファイルを一つも見ずに、同じ意匠へ到達できる粒度で書く。
- 確定している CSS ・マークアップは、文章で要点を述べるだけでなく、コード片としてそのまま載せる。
- 既存ファイルを見て初めて分かった約束事に気づいたら、その場で規約に昇格させる。文書の約束事ならスキルへ、 `portal.html` の約束事ならこの `CLAUDE.md` へ書く。
- 規約の例示が実物と食い違うときは、実物に合わせて規約を書き換え、その方式にした理由も添える。
- 理由 : 規約が実物より古くなると、存在しない構造を前提に作業してしまう。

## git の運用
- `main` へ直接コミットし、 `git push origin main` する。ブランチを切る提案や確認は不要である。
  - 理由 : GitHub Pages が `main` から直接公開しており、ブランチに積むとサイトが更新されない。単一著者の個人サイトで、レビューを挟む相手もいない。
- プッシュがリモートの新規コミットで拒否されたら、 force push せず作業を止めて報告する。
- コミットメッセージは、既存履歴に合わせて英語の命令形で 1 行に書く（例 : `Add article on …` 、 `Update …` 、 `Revise …` 、 `Remove …` 、 `Replace …` ）。文書の追加は、公開まで含めて `… and list it in the portal` のように書いた例がある。
- 同期を頼まれたら、 `git status` の前に必ず `git fetch origin` を実行する。
  - 理由 : `git status` はローカルに残る古いリモート追跡参照と比べるだけなので、上流の変更を見逃す。
- 作業中、自分が触れていないファイルに差分が出ても、確認や警告で作業を止めず、「この差分は私の作業ではない」と事実を一行添えるだけにする。ユーザー本人の手作業であることが多い。
  - 編集の直前にファイルを読み直し、読み込んだ内容の上に変更を重ねる。
- プッシュ後に公開サイトへの反映を確かめるよう頼まれたら、 `gh api repos/morihrkz/reading/pages/builds/latest` を実行し、 `"status":"built"` になるまで繰り返す。
  - `gh` がない PC では、公開 URL を `ctrl+shift+r` で開き、変更が反映されたかを目で確かめる。
  - 公開 URL は `https://morihrkz.github.io/reading/<ファイル名>.html` である（トップは `https://morihrkz.github.io/reading/` ）。ビルドは、プッシュから 10 〜 20 秒で終わることが多い。
  - 同じ URL をブラウザで見直すときは、キャッシュを避けるため `ctrl+shift+r` で再読み込みする。
  - 理由 : プッシュしただけでは、公開サイトが最新だとは限らない。
- 「コミットから push まで一気通貫で」のように、手順の両端を明示して頼まれたら、途中で確認を挟まずに続けて実行する。実行後に、コミットのハッシュと push の出力を示す。
  - 依頼に含まれない操作（ force push 、ブランチの削除など）は、個別に確認する。
- `.gitignore` は `.claude/` ・ `.DS_Store` ・ `INSTRUCTIONS-*.html` ・ `public_URL.txt` を除外している。これらはコミットに含めない。
- コミットを提案する前に、頼まれた編集の範囲より広い見直しを、一度行う。
  - （1）ファイル間のメタ情報（件数、タイトル、他のファイルを指すラベル）の整合。確かめる場所は、「 portal.html の構造」の「件数が載る場所」に挙げた。
  - （2）文書の `<style>` を雛形としてコピーしたときに残る、未使用の CSS クラスや id 。
  - 見つけたものは一覧で示し、削除は承認を得てから行う。

## 検証
- 文書（ `*.html` ）を編集したら、完了を報告する前に、構造検査を実行する。 `div` ・ `section` の開閉の対応と、囲み（ `.point` など）の入れ子を調べる。検出があれば、報告に含める。
  - 実行 : `python $HOME/.claude/scripts/check_html_nesting.py <ファイル>` （引数なしで作業ディレクトリの全文書。 `index.html` は除かれる）。仕様は `~/.claude/scripts/check_html_nesting_spec.md` 。
  - 理由 : 閉じ忘れはブラウザが黙って補うので、見た目では気づかない。
  - 一括作業（意匠の適用、表記の一括変換など）の後も、全文書に対して実行する。
- 見た目や挙動に関わる変更（レイアウト、レスポンシブ、目次のリンクなど）は、 Claude in Chrome で実際に開いて確かめてから、完了を報告する。
  - `navigate` は `file://` を拒否する。作業ディレクトリで `python -m http.server` を一時起動し、 `http://127.0.0.1:PORT/...` 経由で開く。確認後は、サーバーを必ず停止する。
  - レスポンシブの確認幅は、文書は 640px の前後、 `portal.html` は 640px の前後と 1240px の前後である（ 1240px 以上で目次が左に固定される。はみ出しが無いかも見る）。
  - 同一タブでの `location.hash` だけの遷移は、スクリプトを再実行しない。ページ内リンクは、新規タブで完全に読み込んでも確かめる。
- Claude in Chrome が使えない環境(Mac で Safari だけの場合など)では、 WebKit で確かめる。依頼がなくても、完了を報告する前に行う。
  - 実行 : `python $HOME/.claude/scripts/check_layout_webkit.py <ファイル> --shots <スクラッチパッド内のフォルダ>` 。 Mac で `python` がなければ `python3` 、 Windows で `python` がなければ `py` 。 Web サーバーはスクリプトが内側で起動して止めるので、別に起動しない。仕様は `~/.claude/scripts/check_layout_webkit_spec.md` 。
  - 幅は 390 ・ 480 ・ 700 ・ 1200px が既定である。コントラスト比の基準は、文書も `portal.html` も既定の 4.5 でよい。 `--min-contrast 7` は付けない（旧 contrast の基準で、補助の文字などに WARN が出る）。 NG は直し、 WARN は内容を見て判断し、結果を報告に含める。
  - 初回は PC ごとに `--setup` が要る(仮想環境と WebKit の導入。外部からのダウンロードを伴うので、実行の前にユーザーの承認を得る)。未導入だと、終了コード 3 で案内が出る。
  - スクリーンショットは、 `Read` で開いて目視する。数値だけで済ませない。
  - 実機の Safari そのものではなく、 Playwright 付属の WebKit である。細部(フォントなど)は違うことがあるので、最終確認はユーザーが実機で目視する。
- 文書と `portal.html` はライト固定とする。スキルにもダークの仕様はない。新しい文書にもダーク用の変数を入れない。
  - ダークモードの作業を頼まれたら、方針（全体に広げるか、外すか）をユーザーに確認する。

## 文書の内容と表記
- 数字の表記は、 `~/.claude/skills/_shared/notation.md` の「数字」節に従う。
- 文書の主題を書き換えたときは、タイトル一式（ `<title>` ・ `<h1>` ・ `.subtitle` ・メタ情報帯 `.meta` のうち、その文書にあるもの）とファイル名の整合を、次のレビューで自発的に確かめる。 `portal.html` のカード（ `.tag` ・見出し・説明文・ href ）がずれていないかも洗い出す。
  - ファイル名の変更は GitHub Pages の公開 URL を変えるので、リネームの可否は実行前に必ず確認する。
- 新しいファイル名の指定に拡張子が無いときは、ディレクトリの慣例（このリポジトリでは `.html` ）を補って進めてよい。質問で止まらない。拡張子が混在している場合は質問する。
- 新しいファイル名は、小文字の英数字とハイフン（ kebab-case ）で、主題を表す語にする（例 : `shutdown-full-reset.html` ）。

## portal.html の構造
`portal.html` は文書の一覧で、文書とは別の意匠の 1 枚物である（ `<style>` 内蔵、 JavaScript は本文検索と画面操作の補助の 2 本）。 2026-11-27 に、参考資料（ユーザーが置いた `typing-catalog.html` ）の構成にならって、 CSS を portal 専用に書き直した。文書を八つの節に分け、各節の下をカードに並べる。折りたたみ（アコーディオン）、トグルは無い。全節は、検索していないときは常に展開されている。

- 節内のカードの並び順 : 同じ話題の文書を隣に置き、続編・入門は元の文書の直後に置く。同じ話題の中では、公開日の古い順にする。新しい文書を足すときは、末尾ではなく、同じ話題の隣に入れる（最新の追加は `nav.recent` が受け持つ）。
  - 理由 : 追加順のままだと、関連する文書が離れる（例 : 反証可能性の 2 本が 18 枚離れていた）。
- 節は「主題」で分ける。形式（調査・手順書など）は、節ではなくカードの種別タグが受け持つ。
  - 理由 : 主題の節と形式の節を混ぜると、新しい文書の置き場所に迷う。

### 本文検索
冒頭の件数の札（ `ul.stats` ）の直後、 `nav.toc` の前に、検索窓（ `form.search` ）がある。末尾の 1 本目の `<script>` が、入力欄へのフォーカス時に全カードのリンク先を `fetch` し、本文を集めて検索する（実行時に取得する方式）。取得は同時 6 件までで、取得した本文は、同じタブの間だけ `sessionStorage` （キー `portal-search-v1` ）に残す。 `localStorage` にしないのは、文書を更新したときに古い本文で検索されるのを避けるためである。

- 文書を足しても、検索の対象は自動で増える。索引ファイルやビルド工程は無い。カードは `li.card` で、リンク先は同じディレクトリの `*.html` に限る。
- 空白区切りの語をすべて含む文書に絞り、一致箇所の抜粋（ `p.snippet` ）を `<mark>` 付きで出す。語の間の空白は無視する。 Esc で入力を消す。
- 半角英数字 1 文字だけの語は、ほぼ全件に一致するので、検索に使わない（案内を出す）。日本語の 1 文字は検索に使う。
- 検索語は URL の `?q=` に反映され、 `?q=Adabas` のように開くと検索が復元される。結果の並びは、関連度順ではなく、ページ上の並びのままである（節ごとの構成と両立しないため）。
- 絞り込みは `hidden` 属性で行う。節（ `h2` ・ `p.sec-intro` ・ `ul.cards` ）は、中のカードが 1 枚も残らなければ、まとめて隠れる。 `.card` は `display` を指定しているので、 `[hidden] { display: none !important; }` が必要である。
- 検索中は、 `nav.toc` ・ `nav.recent` を隠す（目次のリンク先の節が隠れ、新着は絞り込みの対象外のため）。広い画面では、左に固定した目次も隠れる。
- `file://` で直接開くと `fetch` が失敗する。ウェブサーバー経由（公開 URL や `python -m http.server` ）で開く。
- 検索の対象は `li.card` の `a` の `href` である。スクリプトは `main > h2` を節の区切りとして使うので、節の見出しを `h2` 以外にしない。新着（ `nav.recent` ）の項目を `li.card` にしない（検索の対象に二重に数えられ、絞り込みも崩れる）。

### 画面操作の補助
末尾の 2 本目の `<script>` が、次の三つを受け持つ。検索とは独立していて、消しても検索は動く。

- `/` キーで検索窓へ移る（入力欄の中では効かない）。入力欄の右端に `kbd` の印を出し、フォーカス中と入力後は隠す。
- 目次で、表示中の節のリンクに `a.active` を付ける（ `IntersectionObserver` で `main > h2` を見る）。広い画面の固定目次で効く。
- 600px 以上スクロールすると、右下に「↑」ボタン（ `button#top-btn` ）を出す。各節の末尾の「↑ 目次へ」は、これに置き換えて廃止した。
- ダークの切り替えは入れない（文書がすべてライトで、行き来するたびに明暗が反転するため）。

### 階層とマークアップ
```
main                     # 検索スクリプトが `main > h2` を使うので、 main は残す。節を section で包まない
  p.kicker               # 「ポータル」
  h1                     # 作成文書インデックス
  p.subtitle             # A Reading Room
  ul.stats               # 件数の札。 li を 4 つ :「収録 <b>N</b> 点」「<b>8</b> 節」「Created 日付」「Updated 日付」。 time は使わない
  form.search            # label + div.field（ input#q + kbd「/」） + p#qstatus.search-status
  nav.toc#toc            # 8 節へのページ内リンク（ p.toc-title「目次」+ ol 。 a href="#secN" の中に、名前と span の件数。番号の札は CSS の連番）
  nav.recent             # 新着 5 件（ p.toc-title「新着」+ ul 。 li に time と a 。手書き。 li.card にしない）
  h2#secN                # 節の見出し。 <span class="no">N</span>名前 （番号は札の文字として書く。検索で節が隠れても番号がずれないよう、 CSS の連番にしない）
  p.sec-intro            # 節の説明（1 〜 2 文）。 h2 と合わせて一枚の帯に見える
  ul.cards
    li.card              # span.tag + a + p + span.lang（ lang の中に time ）
  p.endnote              # 末尾の注記
button#top-btn           # 右下の「↑」
script                   # 本文検索
script                   # 画面操作の補助
```
- 新しい文書は、該当する節の `ul.cards` に `li.card` として追加する。合う節がなければ、節（ `h2` ・ `p.sec-intro` ・ `ul.cards` ）と `nav.toc` のリンクを足す。ただし、節の新設は構成の変更なので、先にユーザーへ相談する。
- 1 枚のカードは、次の四つ組である。リンク先が英語の文書には、 `a` と `p` に `lang="en"` を付ける。
  - `span.tag` : 種別の 1 語（下の 7 種から選ぶ）。主題は、節が受け持つ。
  - `p` : 説明文。 2 文・ 150 字程度（英語は 250 字程度）まで。方法の限界は文書に任せ、読者の判断に効く未確認の一句（例 : 公式マニュアル未確認）だけを残す。
  - `span.lang` : 「日本語」「英語」など、本文の言語と、「 ・ 公開 」に続けて公開日（ `<time datetime>` ）。
- 公開日は、その文書を最初にコミットした日である（ `git log --diff-filter=A --format=%as -- <ファイル>` の最も古い日付）。文書を更新しても変えない。最終更新日は、一括の意匠適用で同日になるので使わない。
- 種別は次の 7 種である。種別を増やすときは、先にユーザーへ相談する。

| 種別 | 使う文書 |
| --- | --- |
| 調査 | 公開資料から調べ直した結果のまとめ（製品・企業・業界） |
| 分析 | 論点を立てて検討し、事実と筆者の推論を分けて論じる文書 |
| 解説 | 基礎知識、制度、仕組みを説明する文書 |
| 手順書 | 手を動かすための手順 |
| 資料 | 参照用の表・比較・転載・見本 |
| 要約 | 映像や記事の要約 |
| 記録 | 作業の記録 |

```html
<li class="card"><span class="tag">手順書</span>
<a href="shutdown-full-reset.html">シャットダウンを「再起動」と同じ深さにする設定手順書</a>
<p>説明文（ 2 文・ 150 字程度）。</p>
<span class="lang">日本語 ・ 公開 <time datetime="2026-10-14">2026-10-14</time></span></li>
```
- 新着（ `nav.recent` ）は、公開日の新しい順に 5 件を、手で並べる。文書を足したら、先頭に入れて、古い 1 件を外す。項目は、日付（ `<time>` ）と、カードと同じ見出しのリンクである。
### 件数が載る場所
件数は、すべて手書きで、自動集計されない。文書を足す・移す・外すたびに、次を合わせる。

1. `portal.html` の `ul.stats` の「収録 N 点」と「 Updated 」の日付（ `2026-10-25` のように ISO 形式）。節を増減したら「 N 節」も。「 Created 」は変えない。
2. `portal.html` の `nav.toc` の各リンクの中の `span` （その節のカード数）。
3. `portal.html` の `nav.recent` （新着 5 件。文書を足したときだけ入れ替える）。
4. `README.md` の総数（冒頭と、ファイル構成の `*.html` 行）、節の表の内容（節名と、収録する文書の紹介）。
5. `future-article-themes.md` の対象本数と、本数の集計表。ただし、この文書は基準日時点の記録なので、本数を書き換えず、基準日以降に文書を足した旨を一言添えるにとどめてよい。

カード数と文書数は、次のコマンドで機械的に数えて照合する。 `nav.toc` の数字は、節ごとにカード数と一致するかを見る。

```
grep -o '<li class="card">' portal.html | wc -l                                          # カード数。文書数 - 2 と一致
ls *.html | grep -v -e '^index.html$' -e '^portal.html$' | wc -l                         # 文書数（掲載対象外の 2 件を含む）
grep -c '<time datetime' portal.html                                                     # カード数 + 新着の 5 件
grep -c '<h2 id="sec' portal.html                                                        # 節の数。 ul.stats の「 N 節」と nav.toc の項目数に一致
```
文書ファイルのうち、どのカードからも `href` されていないものがないかも確かめる（掲載対象外の 3 件のうち `index.html` を除く 2 件、 `megumino.html` ・ `color-palette.html` だけが、リンクを持たない）。
カード数は、文書数から 2 件（ `megumino.html` ・ `color-palette.html` ）を引いた数と一致する。

### 意匠の要点
- portal 専用の CSS である（旧 contrast の土台は 2026-11-27 に外した。退避のための上書きの塊も無い）。色は `readable-html-style` の変数名と値をそのまま使い、そこから作った派生（淡い緑の地、半透明の緑の線、影）を足す。色はこれらの変数だけを使う（白の地と、札の文字の白を除く）。書体は指定しない。ライト固定（ `color-scheme: only light` ）。
```css
:root {
  --bg: #f7f8f6; --text: #242522; --muted: #65695f; --accent: #3d5a52; --line: #868a83;
  --box: #eceee7; --mark: #ffe27a; --note-bg: #fff6d6; --note: #d9a400; --must-bg: #fde8e6; --must: #c0392b;
  --surface: #fff;
  --border: #d3d7cd;
  --accent-soft: rgba(61, 90, 82, .10);
  --accent-line: rgba(61, 90, 82, .45);
  --shadow: 0 1px 2px rgba(20, 30, 20, .06), 0 8px 24px -12px rgba(20, 30, 20, .20);
  --side: 300px;
}
```
- 全体の見た目 : 地は `--bg` に右上から淡い緑のにじみ（ `radial-gradient` ）。部品は白の地、 1px の `--border` の枠、角丸 14px 、 `--shadow` の影でそろえる。太い枠や塗りの帯は使わない。
- 冒頭 : `p.kicker` は字間を広げた小さい灰の文字、 `h1` は `--text` から `--accent` へのグラデーションの文字（印刷時は単色）。 `ul.stats` は丸い札で、数字（ `b` ）を緑の太字にする。
- 目次 : 狭い画面では、番号の札（ `--accent` の地に白、 CSS の連番）と件数を持つタイルを、 `auto-fill` の格子に並べる。幅 1240px 以上では、左に固定（幅 `--side` ）した縦の一覧になり、 `main` はその右に寄る。表示中の節は `a.active` （淡い緑の地と、左の緑の線）。
- 節の見出し : `main > h2` と続く `p.sec-intro` を、同じ淡い緑のグラデーションと半透明の緑の枠で、上下に継いで一枚の帯に見せる（ h2 は下の枠なし・上の角丸、 sec-intro は上の枠なし・下の角丸）。番号は `span.no` の札。
- カードは、幅 26rem 以上を 1 列の目安とする格子（広い画面で 2 列）。種別は淡い緑の丸い札。ホバーで枠が緑になり、 2px 浮く。カード全体をクリックできるよう、 `a::after` を `inset:0` に広げ、公開日の行（ `span.lang` ）はカードの下端にそろえる。
```css
ul.cards { list-style: none; margin: 0; padding: 0; display: grid; grid-template-columns: repeat(auto-fill, minmax(min(100%, 26rem), 1fr)); gap: 14px; }
li.card { position: relative; display: flex; flex-direction: column; margin: 0; background: var(--surface); border: 1px solid var(--border); border-radius: 14px; padding: 16px 20px 14px; box-shadow: var(--shadow); transition: border-color .2s, transform .2s; }
li.card:hover { border-color: var(--accent-line); transform: translateY(-2px); }
li.card:focus-within { border-color: var(--accent); outline: 3px solid var(--accent); outline-offset: 2px; }
.card .tag { align-self: flex-start; margin: 0 0 .5rem; padding: 0 .85em; font-size: 1rem; font-weight: 700; line-height: 1.7; color: var(--accent); background: var(--accent-soft); border: 1px solid var(--accent-line); border-radius: 999px; }
.card a { font-size: 1.25rem; font-weight: 700; line-height: 1.5; color: var(--text); text-decoration: none; }
.card a::after { content: ""; position: absolute; inset: 0; border-radius: 14px; }
.card a:focus-visible { outline: none; }
li.card:hover a { color: var(--accent); }
.card p { margin: .4rem 0 .8rem; font-size: 1.1rem; line-height: 1.7; }
.card .lang { margin-top: auto; font-size: 1rem; color: var(--muted); }
```
- ホバーとキーボード操作の表示は、リンク文字ではなくカード全体に付ける（クリックできるのがカード全体のため）。リンク自身の枠線は、 `:focus-within` の枠線と重なるので消している。
- 文字サイズは rem で書く。本文 1.2rem 、カードの説明 1.1rem 、最小の文字は 1rem 。 `main` は `max-width: 1100px` で中央に置く（広い画面では左の目次の右）。
- 動きは `prefers-reduced-motion: reduce` のとき止める。印刷では、目次・検索窓・↑ ボタンを隠す。
- 上記以外の値は、 `portal.html` の `<style>` が正である。この `CLAUDE.md` に全文を写さないのは、写しが古くなって実物と食い違うのを避けるためである。数値を変えたら、上の変数とコード片だけ合わせる。

### 構成についての相談
- 一覧ページが長くなった、分類を見直したい、という相談には、現在の構成（ 8 節・カード）の中でできること（節の分け直し、統廃合、説明文の整理）を先に検討する。折りたたみやタブの導入は、本当に必要になってから提案する。
- 分類軸や構成について見解を求められたら、無難に追認せず、擁護できる点を挙げたうえで問題点を具体的に名指しし、「私ならこうする」と代替案を一つ推す。
  - 提案と実行は分ける。実際に作り直すのは、承認を得てからにする。
  - ユーザーの信条は「変わることを躊躇しない」である。既存の構造を保つことより、より良い形への作り直しを優先する。
