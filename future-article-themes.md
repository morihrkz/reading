# 「作成文書」次の文書テーマ

**文書名** : `future-article-themes.md`
**基準日** : 2026 年 11 月 21 日（前回は 11 月 14 日。この間に文書が 22 本増え、 1 本が削除され、 1 本が掲載対象外になり、 portal の節が組み替わった）。なお、基準日の後に `solo-income-with-ai-japan.html` を第 5 節へ、 `iran-dprk-human-rights-votes.html` を第 2 節へ、 `us-parties-china-russia-trilateral-summit.html` を第 2 節へ加えた（ 2026 年 11 月 22 日・ 23 日・ 25 日）。また、 2026 年 11 月 25 日に、 `elder-housing.html` を大幅に改訂し（静岡市などの自治体の取組みの章と、参考文献を追加。 contrast の意匠へ変更。以下の出典・限界に関する 82 ・ 108 ・ 199 行の記述は、改訂前のまま）、 `suginami-nursing-home-address-change.html` を廃止して削除した（第 6 節。以下の本数と集計、および 53 行・ 111 行の記述は、削除前のまま残してある）。以下の本数と集計は、基準日時点のままである
**対象** : 『作成文書――A Reading Room 』の、 portal に掲載された文書 67 本・ 8 節。 `index.html` ・ `megumino.html` ・ `autumn-colors.html` ・ `color-palette.html` の 4 件は、今も将来も portal に載せない（ユーザーの決定。 `CLAUDE.md` に記載）。 `portal.html` は一覧そのもので、文書の数に入れない。ファイルは、この 4 件のうち `index.html` を除く 3 件を含め、文書が 70 本ある。
**増減の内訳** : 前回の 47 本に、 22 本が加わった。そこから、廃止した 1 本（ `superiority-social-comparison.html` ）と、掲載対象外にした 1 本（ `color-palette.html` ）を引くと、 67 本になる（ 47 + 22 − 1 − 1 ）。 `disagreement-and-sense-of-superiority.html` は、 11 月 19 日に追加して同日に廃止したので、差し引きに入らない。
**削除の注記** : 2026 年 11 月 19 日に、 `superiority-social-comparison.html` と `disagreement-and-sense-of-superiority.html` を廃止した（別のリポジトリで、 2 本を統合した新しい文書を作ったため）。前回までの本稿にあった、これらへの言及は、この版で外した。
**役割** : 作成文書の現状を診断し、次に書く・直す文書を優先順に提案する。新規の候補ごとに、執筆の前に決めておくこと（置き場所、入口、論点の分担、確度の見通し、接続先）を示す。

**この文書の根拠**

- **読んだ範囲** :
  - 前回までの読み（ 10 月 27 日、 11 月 6 日、 11 月 14 日）を引き継いだ。
  - 今回は、全 70 文書の HTML を機械的に走査した（本数、字数、見出しの種類、冒頭部の部品、文書どうしのリンク、最初のコミット日）。
  - そのうえで、状況が動く 5 本（ `us-midterm-2026.html` 、 `trump-omar-midterms-2026.html` 、 `japan-economic-sphere-table-2026.html` 、 `election-schedule-japan.html` 、 `ai-industry-comparison.html` ）と、 11 月 14 日以降に増えた 22 本すべて、 11 月 14 日までの追加分のうち 6 本（ `active-cyber-defense.html` 、 `kaitori-shop-fc-and-pawnshop.html` 、 `consumption-tax-cut-walkouts.html` 、 `russia-authoritarian-consolidation.html` 、 `industrial-designers-and-architecture.html` 、 `cross-country-statistics-comparability.html` ）について、題名、リード、メタ情報帯、見出し、「限界」「未確認」「確度」の節（長い節は冒頭の 700 〜 1,400 字まで）を読んだ。
  - `portal.html` のカードと節の構成、 `README.md` 、 `CLAUDE.md` 。
- **測った範囲** : 字数は、各文書の本文からタグ・スタイル・スクリプト・空白を除いて数えた（目次と表を含む）。見出しの種類は、 `h2` と `h3` の文字列で判定した（本文中の言及は数えない）。したがって、前回までの件数とは、数え方が少し違う。節への割り当ては `portal.html` の現状による。
- **読んでいない範囲** :
  - どの文書も、全文の通読はしていない。限界の節の読みも、冒頭までである。
  - 文書が書く外部の事実（統一地方選の法案の成立、楽天の再編の完了、 Anthropic の上場、 Alaska の議席の確定など）は、外部で確かめていない。 3 章と 5 章に出てくる「いまの状況」は、すべて、文書自身の記述（最後の更新日時点）である。
  - 新規候補の接続先は、「本文で確認済み」と「論理上の接続」（主題が隣り合うだけで、本文での確認は未了）を分けて書く。後者は、設計の段階で本文を読んで確かめる。

---

## 目次

1. [作成文書の現状](#1-作成文書の現状)
2. [作成文書に共通する書き方](#2-作成文書に共通する書き方)
3. [宿題はどこにあるか](#3-宿題はどこにあるか)
4. [候補を選ぶ基準](#4-候補を選ぶ基準)
5. [次に書く・直す文書と優先順](#5-次に書く直す文書と優先順)
6. [新規候補ごとの設計](#6-新規候補ごとの設計)
7. [保留中のテーマ](#7-保留中のテーマ)
8. [文書を足すときの手順](#8-文書を足すときの手順)

---

## 1. 作成文書の現状

`portal.html` は、 67 本を八つの節に分けて並べている。 11 月 12 日の再編（コミット `411a55f` ）で 8 節になり、 11 月 21 日に、節の内容を組み替えた。

- 旧第 8 節（資料・見本）を解消した。形式で分けた節は、主題の軸と食い違うためである。 `dl-tag.html` は第 5 節へ移し、 `color-palette.html` は掲載対象外にした。
- 24 枚あった旧第 7 節を、第 7 節（思考・論証・言語）と第 8 節（文化・歴史・科学・スポーツ）に分けた。
- 第 5 節と第 6 節の境界を直した（ OS の設定と、サイトの移行は第 5 節）。
- 節内のカードは、同じ話題を隣に置き、続編は元の文書の直後に置き、話題の中では公開日の古い順に並べ直した（規則は `CLAUDE.md` ）。

前回（ 11 月 14 日）から追加された文書は、次の 22 本である。

- 11 月 14 日 `china-russia-aligned-states`
- 11 月 15 日 `godzilla-films-chronological-list` ・ `gamera-films-chronological-list` ・ `venezuela-lvbp-guide`
- 11 月 16 日 `countries-without-state-form-words` （最初は `single-word-country-names` で、同日に改名した）・ `mikitani-consumption-tax-and-yen` ・ `abstraction-concreteness-math-law` ・ `the-plural-in-country-names` ・ `dental-clinics-rise-and-fall` （翌 17 日に、中立的な統計の概観へ書き直した）
- 11 月 17 日 `female-category-gender-identity-sports` ・ `polygyny-legalization-pro-con`
- 11 月 19 日 `motor-vs-engine-english` ・ `suginami-nursing-home-address-change` （同日に 3 回改訂した）
- 11 月 21 日 `elder-housing` ・ `japan-industrial-products-strength` ・ `modern-contemporary-periods` ・ `strawman-fallacy` ・ `logic-argumentation` ・ `writing-techniques` ・ `falsifiability-introduction` ・ `if-adopted-at-one` ・ `review-jibun-toka-nai-kara` （ wafu の意匠で、まとめて追加した）

| 節 | 見出し | 掲載数 | 平均字数 |
| :---: | :--- | :---: | :---: |
| 1 | 日本の政治・制度 | 5 | 4,568 |
| 2 | 米国・国際 | 8 | 9,545 |
| 3 | 企業・産業・経済 | 11 | 8,675 |
| 4 | FPV ドローンと周辺機器 | 5 | 8,274 |
| 5 | AI ・パソコン・ウェブのツール | 9 | 10,343 |
| 6 | 暮らし・介護・健康 | 5 | 10,829 |
| 7 | 思考・論証・言語 | 15 | 7,997 |
| 8 | 文化・歴史・科学・スポーツ | 9 | 10,028 |
| | **合計** | **67** | **8,857** |

この表から、次の五つが読み取れる。

- **節の厚さ** : 最少の節も 5 本あり、一本だけの節はなくなった。最も厚いのは第 7 節（ 15 本）で、第 3 節（ 11 本）が続く。 24 本あった節を分けたので、偏りは前回より小さい。
- **字数の差** : 第 1 節は平均 4,568 字で、最も短い。第 6 節は 10,829 字で、最も長い。第 1 節の 5 本は、時事の整理が中心で、短くまとまっている。
- **更新が前提の文書** : `us-midterm-2026.html` は、 11 月 4 日の追加後、 11 月 6 日 、 11 日 、 12 日と更新されている。 11 月 12 日の更新時点で、上院は Alaska だけが未確定、下院は 15 議席が未確定（ 11 月 10 日時点）と書く。時事の文書は、情報の時点が価値を決める（ 3 章）。
- **英語の文書と文書どうしのリンク** : 英語の文書は、 `us-midterm-2026.html` と `us-election-lexicon.html` の 2 本である。本文中のリンクで他の文書へつなぐ例は、 3 組だけで、すべて片方向である（ `adabas-overview.html` → `software-ag-overview.html` 、 `motor-vs-engine-english.html` → `electric-motor-guide.html` 、 `us-election-lexicon.html` → `us-midterm-2026.html` ）。 `trump-omar-midterms-2026.html` と `us-midterm-2026.html` の間には、リンクがない。
- **反証可能性と論証の系統** : 反証可能性の 2 本、論理学入門、藁人形論法、文章表現技法が揃い、第 7 節に「論証」の系統ができた。本文中のリンクでは、まだつながっていない。

---

## 2. 作成文書に共通する書き方

見出しと導入部、限界の節を通して読むと、作成文書には共通する書き方がある。新しい文書も、この書き方を満たせる主題を選ぶ。件数は、掲載の 67 本についてのものである。

- **出典を挙げる** : 「出典」「参考文献」を見出しに持つ文書は、 67 本のうち 57 本である（英語の見出し Sources などを含む）。持たない 10 本は、手順書・環境移行・実務記録（ `claude-code-migration.html` 、 `shutdown-full-reset.html` 、 `static-site-migration.html` ）、日程表（ `election-schedule-japan.html` ）、用語集（ `us-election-lexicon.html` ）、技術解説（ `dl-tag.html` ）、解説（ `electric-motor-guide.html` 、 `elder-housing.html` 、 `japan-industrial-products-strength.html` ）、筆者の整理（ `abstraction-concreteness-math-law.html` ）である。見出しがないだけで、本文に出典を書いている場合は、数えていない。
- **限界を書く** : 「限界」を見出しに持つ文書が 18 本、メタ情報帯に【方法と限界】を置く文書が 33 本ある。「確認できていないこと」「未確認」「確かめられなかったこと」を見出しにする文書も 9 本ある。いずれかを持つ文書は 47 本で、残る 20 本は、どれも持たない（ 3 章の（ 0 ））。
- **事実と解釈を分ける** : `chudo-kaikaku-rengo-analysis.html` 、 `icc-akane-us-sanctions.html` 、 `fpv-maneuver.html` 、 `sony-ip-shift.html` （動機や因果に踏み込む箇所を「と考えられる」と明示）などが、「確認できた事実」と「筆者の推論・解釈」を分けて書くと宣言している。新しい文書では、 `china-russia-aligned-states.html` （「筆者の見立てでは」）、 `mikitani-consumption-tax-and-yen.html` （三つの仮説と、確かめられたこと・られていないことの区別）、 `female-category-gender-identity-sports.html` （「線引きの試案」）が同じ書き方をする。確度を段階で示すものもある（ `election-schedule-japan.html` の「この文書の確度」は高い・中程度・低い、 `dji-manual-mode-note.html` の「確度について」）。
- **時点を明記する** : 「時点」の語を本文に持つ文書が 40 本ある。作成日、調査日、情報基準日、取得日、確認日のいずれかをメタ情報帯に置く。
- **結論を先に書く** : 「要点」「結論」「要旨」「要約」の節を持つ文書が 27 本ある。このほか、リードで「結論から述べる」「結論から言う」と書く文書がある（ `election-schedule-japan.html` 、 `the-plural-in-country-names.html` 、 `motor-vs-engine-english.html` 、 `female-category-gender-identity-sports.html` 、 `industrial-designers-and-architecture.html` ）。
- **実機・原典で確かめていないことを明記する** : `shutdown-full-reset.html` （「実機での動作確認は未実施」）、 `emdash-learning-guide.html` （「手順を実機で通して検証してはいない」）、 `mac-vs-windows-differences.html` （ FPV ゲームを「実機で動かして確かめていない」）、 `suno-mcp-guide.html` （「実機では未検証」）。書評の `review-jibun-toka-nai-kara.html` は、出版社の公開情報と著者インタビューを手がかりにして、本文を読んだかのような引用や評価をしないと書く。
- **筆者の整理であることを明記する** : `abstraction-concreteness-math-law.html` は、「筆者による整理であり、学習指導要領や法学の文献で一つずつ裏付けたものではない」と、メタ情報帯に書く。

冒頭部は、 67 本のうち、 `.kicker` が 45 本、 `.subtitle` が 46 本、 `.lede` が 48 本、 `.meta` が 19 本にある（ HTML の走査による）。この文書の対象外とし、揃えるかどうかは別に判断する（ `CLAUDE.md` は、頼まれていないのに揃えないと定める）。

---

## 3. 宿題はどこにあるか

作成文書は、自分が確かめきれなかったことを、文書の中に書いている。語の出現数から空白を推し量るのではなく、**文書が自分で書いた未確認の点**が、次の文書の最も確かな根拠になる。本文を読んで、解く手段で四つに分けた。

**（ 0 ）限界の記述が見つからない、または、まだ読んでいない文書**

限界の見出しも、【方法と限界】も、「確認できていないこと」の見出しもない文書が 20 本ある。

`claude-code-migration.html` ・ `cloud-market-ai-analysis.html` ・ `dl-tag.html` ・ `elder-housing.html` ・ `electric-motor-guide.html` ・ `gamera-films-chronological-list.html` ・ `godzilla-films-chronological-list.html` ・ `if-adopted-at-one.html` ・ `japan-economic-sphere-table-2026.html` ・ `logic-argumentation.html` ・ `obsidian-cli-guide.html` ・ `plateau-ai-workflow-guide.html` ・ `shutdown-full-reset.html` ・ `static-site-migration.html` ・ `strange-novels-of-japan.html` ・ `strawman-fallacy.html` ・ `the-zone-fpv-simulator.html` ・ `us-election-lexicon.html` ・ `us-midterm-2026.html` ・ `writing-techniques.html`

このうち、中身を読んだ文書では、限界にあたる記述が別の見出しに入っている（ `japan-economic-sphere-table-2026.html` の「確認できなかった項目、基準日以後に変わりうる点」、 `us-midterm-2026.html` の「 Sources and Editorial Notes 」）。

| 文書 | 現状 | 次に読むこと |
| :--- | :--- | :--- |
| `elder-housing.html` ・ `japan-industrial-products-strength.html` | 出典の見出しがない（後者は【方法と限界】を持つ） | 本文に出典があるか。なければ、出典と限界を足す |
| `logic-argumentation.html` ・ `strawman-fallacy.html` ・ `writing-techniques.html` | 参考文献はあるが、限界の節も【方法と限界】もない | 事例・技法の選び方の限界を足すか |
| `godzilla-films-chronological-list.html` ・ `gamera-films-chronological-list.html` | 「この文書の範囲と数え方」の節があり、終章に今後の作品（『ゴジラ -0.0 』『 GAMERA -Rebirth- 』）の位置づけがある | 新作の公開で古びる。公開時に追記する |
| `suginami-nursing-home-address-change.html` | 【方法と限界】がある。本文は 11 月 19 日に 3 回改訂 | 限界の内容。届出を済ませたあとに、実際の流れを追記できるか |
| `consumption-tax-cut-walkouts.html` ・ `venezuela-lvbp-guide.html` | 「確認できなかったこと」の見出しがある | 限界の内容（本文は未通読）。前者は、「これから」に日付で動く記述がないか |
| `if-adopted-at-one.html` | 【本稿の射程】で、思考実験であり実証研究でないと断る | 追加の確認は不要 |

- `electric-motor-guide.html` は、 Git の履歴では `electric_motor_guide.html` で追加された。 `CLAUDE.md` は「アンダースコア区切りは改名済み」と定める。ファイル名の改名は公開 URL を変えるため、実行前に確認が要る（すでに改名済みなら、旧 URL は使えない）。

**（ A ）本人の実機・実体験・実読でないと閉じられないもの**

| 文書 | 確認できていないこと（本文の記述） |
| :--- | :--- |
| `shutdown-full-reset.html` | 実機での動作確認は未実施（仕様に基づく手順）。 |
| `emdash-learning-guide.html` | 手順を実機で通して検証してはいない。画面の文言や選択肢の名前が実際と違うかもしれない。 |
| `mac-vs-windows-differences.html` | FPV ゲームを実機で動かして確かめていない。 Mac での送信機の認識も確認できなかった。 |
| `ahamo-migration-guide.html` | お申込みサポートに来店予約が必須か、所要時間、支払い方法など。手続きを済ませた時点で、実際の流れを追記できる。 |
| `suno-mcp-guide.html` | 作成時点（ 2026-10-31 ）で、 MCP の追加、 Suno や Claude へのサインイン、曲の生成を一つも行っていない。承認画面の文言、接続状態の表示、一曲と頼んだときにつくられる曲数とクレジットの消費量も未確認。 |
| `nexradio-dcs-gimbal.html` | `TX16S MK II` の実機と、取付ガイド（ UART4 の既定設定、ケーブル長、コネクタ形状）との照合。 |
| `review-jibun-toka-nai-kara.html` | 出版社の書誌情報・紹介文・目次と、著者インタビューを手がかりにした書評で、本文を精読していない。本を読めば、論証の細部を確かめられる。 |

**（ B ）一次資料に当たれば閉じられるもの**

| 文書 | 確認できていないこと（本文の記述） |
| :--- | :--- |
| `fpv-maneuver.html` | FPV が目視外飛行にあたるか（二次的な資料のみ）。電波法上の免許・資格の扱い。小型無人機等飛行禁止法の法令本文と、改正の施行日。 |
| `handlebar-rc-japan-import.html` | 日本向けの発送の可否、関税率の区分。技適番号の照合。実験等の特例制度の現在の対象規格。 |
| `nexradio-dcs-gimbal.html` | BETAFPV と RadioMaster の公式ページが取得制限（ HTTP 429 ）で再確認できず、本体仕様は報道記事との照合にとどまる。ジンバルの価格（約 32 米ドルか 39.99 米ドルか）と販売単位（ 1 個か 2 個か）、本体の価格（ 135.99 米ドルとする検索結果がある）、 RadioMaster 純正ジンバルの国内価格。 |
| `adabas-overview.html` / `software-ag-overview.html` / `essbase-history.html` | **三本が共通して**、 1990 年代の日本での販売体制・日本法人の役割・日本語版の初出を、確認できていない。 `essbase-history.html` は「当時の日本の業界誌や、両社の発表資料に当たる必要がある」と書く。 |
| `adabas-overview.html` | Natural 自体の詳しい来歴（専用の百科事典の記事が取得できなかった）。 |
| `dji-manual-mode-note.html` | DJI 公式の取扱説明書の本文。 Neo 2 に初代 Neo と同じ姿勢制限の設定があるか。 |
| `icc-akane-us-sanctions.html` | 米国務省・財務省の原文書（直接確認できなかった）。 |
| `tire-size-and-outer-diameter.html` | JATMA と ETRTO の規格書そのもの。読んだ国内の条文は 2013 年の版で、現行のものではない。 |
| `aave-mle-expanded-study.html` | Labov 、 Fricker 、 Green 、 Cheshire らの原典の全文は読んでいない。日本語の辞書が「黒人英語」をどう定義しているかも未確認。 |
| `falsifiability-rabbit-fossil.html` | ホールデンの逸話の一次資料。要確認の数値（初期の四足動物の年代、ドウソノラグスの年代、ホモ・サピエンスの年代、炭素 14 とウラン 238 の使い分けの範囲）。ウサギ目の起源は、化石と分子系統とで食い違い、決着していない。 |
| `new-condos-in-japan.html` | 購入者の層ごとの割合、個人投資家と法人の占める割合、 2025 年に 1 億円以上の住戸が東京 23 区の発売戸数に占めた割合、海外居住者の取得割合の通年・区別の数字（本文は 2025 年 1 〜 6 月の値）。 |
| `bluejays-2026-decline.html` | 接戦の成績、リーグ全体の得点環境、予測システムの数字、守備・走塁の指標。出典が媒体名の列挙にとどまる箇所。 |
| `suno-mcp-guide.html` | Suno MCP の生成の上限と 1 曲あたりのクレジット消費量、 Suno 側で許可を取り消す方法、日本語の歌詞への対応、 Code タブでのカスタムコネクタの追加手順など（「調べても確認できなかった事項」として本文が列挙）。 |
| `china-russia-aligned-states.html` | 国連の公式の投票記録と条約の本文は、直接には読んでいない（ Wikipedia と UN Project 経由）。アルメニアの CSTO の議決権停止（ 2026 年 11 月 11 日）の一次資料。シリアの反対票の背景。 |
| `countries-without-state-form-words.html` | 出典は英語版 Wikipedia の表とネパールの報道だけ。国連の名簿、各国の憲法、各国政府の公式表記は未確認。ネパールの閣議の日付（ 2020 年 9 月 27 日とする情報がある）。 |
| `mikitani-consumption-tax-and-yen.html` | X の投稿の原文（報道を経由して引用している）。三木谷氏の動機、楽天の財務への影響の大きさ、食料品が楽天市場の売上に占める割合。 |
| `abstraction-concreteness-math-law.html` | 学習指導要領と法学の文献での裏づけ（筆者の整理として書いてある）。 |
| `active-cyber-defense.html` | 法令、内閣官房・内閣府の資料での確認（日本語の解説記事 2 本と英語の記事 2 本に依拠）。通信監視の本格化の時期が、日本語記事は「 2027 年秋」、英語記事は「 2027 年」で食い違う。 |
| `dental-clinics-rise-and-fall.html` | 初期投資の目安は、公的統計ではなく事業者の記事による。需給推計は、厚生労働省のワーキンググループが検討中の資料で、最終の報告は別に確認が要る。 |

**（ C ）時間が経たないと閉じられないもの**

| 文書 | 確認できていないこと（本文の記述） |
| :--- | :--- |
| `japan-economic-sphere-table-2026.html` | 楽天の再編は 2026 年 10 月 1 日の効力発生を予定していた。基準日の時点で、完了した資料を確認できていない。 PayPay の上場後の株主構成、 au じぶん銀行の完全子会社化の完了、 7iD の PayPay ID への統合の時期なども未確認。 |
| `trump-omar-midterms-2026.html` | 「投票日が近く、状況は日々動いている。この記事は 10 月 24 日までの報道に基づく」。投票日（ 11 月 3 日）はすでに過ぎている。 |
| `us-midterm-2026.html` | 11 月 12 日の更新時点で、上院は Alaska が未確定、下院は 15 議席が未確定（ 11 月 10 日時点）。得票率は途中経過で、出典の取得時刻がそろっていない。 AP の数字は、二次的なサイトを経由している。 CNN のページは直接取得できず、見出しと検索結果の要約による。 |
| `election-schedule-japan.html` | 統一地方選の日付は閣議決定された法案に基づき、法案の成立は未了。 2028 年以降の投票日は未定。 |
| `ai-industry-comparison.html` | 2026 年 11 月 6 日に更新した。まだ動く点は、 Anthropic の上場の成否（ WSJ によれば 11 月 16 日の週が目標）、 Gemini 4 Carbon の一般提供、 Muse Wonder の Muse アプリへの展開、 Perplexity と OpenAI の資金調達の成立。 Meta の新モデルの性能値は暫定的なものとして読む必要がある。 |
| `suno-mcp-guide.html` | Suno MCP はベータ版で、画面の名前や手順は変わりうる。 |
| `nexradio-dcs-gimbal.html` | 日本国内の取り扱いが確認できていない。精度・寿命の独立したレビューは見つかっていない。 |
| `china-russia-aligned-states.html` | 数は動く（シリアの政権交代、アルメニアの CSTO 参加の凍結、ベネズエラのマドゥロ大統領の拘束）。 |
| `active-cyber-defense.html` | 2026 年 10 月 1 日に主要部分が施行され、通信監視の本格化は 2027 年の見込み。 |

---

## 4. 候補を選ぶ基準

次の六つを満たすかどうかで、候補を選ぶ。

1. **宿題との対応** : 3 章の宿題を閉じるものを先に置く。新規の主題は、その次にする。
2. **期限** : 基準日を過ぎて古びた記述、まもなく状況が変わる記述は、他の候補より先に直す。
3. **書き方の適合** : 2 章の書き方（事実と解釈の分離、限界の節、出典、時点の明記）を満たせるか。出典が取れない主題は、設計の前に事前調査をして、取れる見通しを確かめる。
4. **入口** : 手元の出来事や、すでにある文書の続きから入れるか。
5. **重複の回避** : 既存の文書に同じ論点がないか。近い文書があれば、論点の分担を設計に書く。
6. **接続** : 既存の文書との関係を、本文で確かめられるか。確かめられない接続は、「論理上の接続」と書く。

節については、次の規則を置く。

- 節は、二本以上で立てる。一本だけの節は、分類ではなく目印にしかならない（ 11 月 21 日の組み替えで、すべての節が 5 本以上になった）。
- 新しい文書は、まず既存の節に収まるかを考える。節の新設は構成の変更なので、先にユーザーへ相談する（ `CLAUDE.md` の規定）。
- 節内では、同じ話題の文書を隣に置き、続編・入門は元の文書の直後に置く。同じ話題の中では、公開日の古い順にする（ `CLAUDE.md` の規定）。

---

## 5. 次に書く・直す文書と優先順

| 順位 | 種別 | 対象 | 節 | きっかけ | 判断 |
| :---: | :---: | :--- | :---: | :--- | :--- |
| 1 | 更新 | `japan-economic-sphere-table-2026.html` | 3 | 楽天の再編の効力発生予定日（ 2026-10-01 ）から、 7 週間以上が過ぎた | 今すぐ着手できる。「確認できなかった項目」を、一次情報で埋める |
| 2 | 更新 | `trump-omar-midterms-2026.html` | 2 | 投票日（ 2026-11-03 ）が過ぎ、結果は `us-midterm-2026.html` が扱っている。本文の時点は 10 月 24 日のままで、二つの文書の間にリンクもない | 結果の確定を待たずに、分担を決められる。 5 章末の「順位の考え方」に案を書いた |
| 3 | 締め | `us-midterm-2026.html` | 2 | 11 月 12 日の更新で、残る未確定は上院の Alaska と、下院の 15 議席（ 11 月 10 日時点）まで絞られた | 結果が確定した時点で基準日を固定し、更新を止める。それまでは、更新のたびに取得時刻を明記する |
| 4 | 更新 | `election-schedule-japan.html` | 1 | 統一地方選の法案の成立が未了 | 成立が報じられた後に着手する |
| 5 | 追記 | `shutdown-full-reset.html` 、 `emdash-learning-guide.html` 、 `mac-vs-windows-differences.html` 、 `suno-mcp-guide.html` 、 `nexradio-dcs-gimbal.html` | 5 ・ 5 ・ 5 ・ 5 ・ 4 | 五本が、実機で確かめていないこと、または実機との照合が済んでいないことを明記している | 本人の実機でしか閉じられない。確認できた分だけ追記し、未確認は未確認のまま残す |
| 6 | 追記 | `review-jibun-toka-nai-kara.html` | 7 | 公開情報だけで書いた書評で、本文を精読していない | 本を読んだうえで、「方法と限界」と第 4 章の論点を見直す。読むまでは、現状の書き方を保つ |
| 7 | 確認 | `dl-tag.html` | 5 | メタ情報帯が「元の記事」の URL を示し、題名に外部サイトの名前が入っている | 本文を読み、転載か、要約・再構成かを確かめる。転載なら、権利と出典の表記を整えるか、自分の言葉で書き直す |
| 8 | 確認 | `elder-housing.html` ・ `japan-industrial-products-strength.html` ・ `abstraction-concreteness-math-law.html` | 6 ・ 3 ・ 7 | 「出典」「参考文献」の見出しがない（ 2 章） | 本文に出典があるかを確かめ、なければ足す。 `abstraction-concreteness-math-law.html` は、筆者の整理と断っているので、足すかどうかを先に決める |
| 9 | 新規 | 日本で FPV ドローンを飛ばすための制度の整理 | 4 | `fpv-maneuver.html` と `handlebar-rc-japan-import.html` が、半分ずつ扱って一次資料を確かめきれていない | 準備は中。 6.1 節 |
| 10 | 新規 | プロジェクトの `CLAUDE.md` は何を変えるのか | 5 | `claude-code-migration.html` は「移す」話で、「何を書くか」の文書はない | 準備は軽。 6.2 節 |
| 11 | 事前調査 | 1990 年代の日本での Software AG ・ Adabas ・ Essbase の販売 | 3 | 三本が共通して未確認と書く | 準備は重。見つかる見通しを先に確かめる。 6.3 節 |
| 12 | 定期更新 | `ai-industry-comparison.html` | 3 | 本文が「製品名・モデル名・提供条件が短期間で変わる」と述べる | 2026-11-06 に更新した。次の節目は、 Anthropic の上場、 Gemini 4 Carbon の一般提供、 Muse Wonder の Muse アプリへの展開。頻度は本人が決める |

**順位の考え方**

- 1 から 4 は、期限のある更新である。 1 は予定日が過ぎて 7 週間以上経ち、すでに古びている可能性がある。 2 は、投票日が過ぎて前提が変わった。 3 は、一つの文書の締め方の問題で、確定を待つ。 4 は、起きるべきことが起きるのを待つ。そのため、着手できる時期が異なる。
- 2 の案 : `trump-omar-midterms-2026.html` は、「名指しの意図と世論」を選挙前の報道で整理した記録として、 10 月 24 日の時点を残す。その上で、冒頭に「結果は `us-midterm-2026.html` を参照」という一文とリンクを足し、 `us-midterm-2026.html` の側にも逆向きのリンクを置く。結果と照らして論旨を書き直すのは、次の段階である。時点を残す理由は、選挙前の見立てと結果とを混ぜないためである。
- 5 は、書き足すというより、確かめた結果を戻す作業である。実機が要るので、本人にしかできない。
- 6 は、書評の信頼性に関わる。現状は、読んでいないことを明記しているので、誤りではない。読んだあとに、引用と評価を本文に基づくものへ置き換えられる。
- 7 は、他者の記事との関係を確かめる作業である。本文を読んでいないため、現時点では転載とも要約とも判断していない。
- 8 は、見出しの有無を数えただけの指摘である。本文に出典が書かれていれば、見出しを足すだけで済む。
- 9 から 11 は新規である。 9 は、シミュレータ（ `the-zone-fpv-simulator.html` ）、機体（ `dji-manual-mode-note.html` ）、送信機の輸入（ `handlebar-rc-japan-import.html` ）、送信機の換装（ `nexradio-dcs-gimbal.html` ）と続く節に、「飛ばすための手続き」という欠けた一段を足す。
- 11 は、 3 章の（ B ）で三本が共通して未確認とした点を、まとめて閉じる試みである。ただし、これまでの検索では情報が出なかったので、成果が出る保証がない。先に事前調査をして、書ける見通しを確かめてから、文書にするかを決める。
- 12 は、一度きりの更新ではなく、運用の話である。頻度や基準日は、本人が決める。更新したら、 `portal.html` のカードの説明文にある基準日も合わせる（ 8 章）。
- 3 章の（ B ）にある新しい文書の宿題（ `china-russia-aligned-states.html` 、 `countries-without-state-form-words.html` 、 `mikitani-consumption-tax-and-yen.html` など）は、一次資料に当たる作業である。個別の順位は付けず、各文書を更新するときに、まとめて閉じる。

---

## 6. 新規候補ごとの設計

各候補は同じ項目で書く。接続先は、本文で確認したものと、論理上のものを分けて示す。

### 6.1 日本で FPV ドローンを飛ばすための制度の整理

- **仮題** : 『日本で FPV ドローンを飛ばすまでに確かめること――航空法、電波法、小型無人機等飛行禁止法を、一次資料で順にたどる』
- **置き場所** : 4 FPV ドローンと周辺機器。節の中の位置は、 `fpv-maneuver.html` の隣に置く。
- **入口** : 節の五本は、操縦の仕組み（ `fpv-maneuver.html` ）、練習（ `the-zone-fpv-simulator.html` ）、機体と操縦モード（ `dji-manual-mode-note.html` ）、送信機の輸入（ `handlebar-rc-japan-import.html` ）、送信機の換装（ `nexradio-dcs-gimbal.html` ）の順に、実際に飛ばす手前まで来ている。足りないのは、「どこで、何を済ませれば飛ばしてよいのか」である。
- **問いと骨格** : 機体の重さと種類による規制の範囲、機体登録とリモート ID 、飛行の場所と方法の規制、電波法（技適と免許・資格）、小型無人機等飛行禁止法の対象施設を、飛ばすまでの順に並べる。 FPV 特有の論点（ゴーグルを着けた飛行が目視外飛行にあたるか、補助者の扱い）を一つの章にまとめる。
- **論点の分担** : 技適と輸入の可否は `handlebar-rc-japan-import.html` 8 章に任せる。この文書は、国内で飛ばす側に絞り、輸入の議論には入らない。 `fpv-maneuver.html` 7 章の概説を、一次資料で確かめ直す形にする。 `nexradio-dcs-gimbal.html` 6 章「日本国内の流通状況と法規」との重なりは、設計の段階で本文を読んで、分担を決める。
- **確度の見通し** :

| 主張 | 確度 |
| :--- | :---: |
| 機体登録とリモート ID の要件 | 要確認（国土交通省のページは `fpv-maneuver.html` が出典に挙げるが、法令本文との照合は未了） |
| FPV 飛行が目視外飛行にあたるか | 未決（二次的な資料のみ。 `fpv-maneuver.html` の限界） |
| FPV 機の操縦に電波法上の免許・資格が要るか | 要確認（一次資料で未確認。 `fpv-maneuver.html` の限界） |
| 小型無人機等飛行禁止法の対象施設と、改正の施行日 | 要確認（法令本文・警察庁の資料が未確認。 `fpv-maneuver.html` の限界） |
| 実験等の特例制度の現在の対象規格 | 未確認（ `handlebar-rc-japan-import.html` の限界） |

- **接続（本文で確認済み）** : `fpv-maneuver.html` （ 7 章「日本の制度と安全」、 8 章「この記事の限界」）、 `handlebar-rc-japan-import.html` （ 8 章「電波法の壁」、 10 章「この記事の限界」）。
- **接続（論理上の接続）** : `dji-manual-mode-note.html` （機体と操縦モード。 EU の速度制限の記述はあるが、「航空法」「電波法」の語は出てこない）、 `the-zone-fpv-simulator.html` （実機の前の練習）、 `nexradio-dcs-gimbal.html` （見出しに「日本国内の流通状況と法規」があるが、本文は未読）。
- **資料** : 国土交通省、総務省、警察庁の公式ページと法令本文。書誌と条文は、公開前に一次資料で確かめる。
- **リスク** : 法令は改正で変わる。時点を冒頭に明記し、「個別の法的助言ではない」と書く（既存の二本と同じ）。手続きの網羅を目指すと、本の分量になる。「飛ばすまでに確かめること」の順にたどる文書に絞る。

### 6.2 プロジェクトの `CLAUDE.md` は何を変えるのか

- **仮題** : 『プロジェクトに `CLAUDE.md` は要るのか――あるリポジトリと、無いリポジトリの比較から』
- **置き場所** : 5 AI ・パソコン・ウェブのツール。 `claude-code-migration.html` の隣に置く。
- **入口** : 手元の二つのリポジトリは、一方に `CLAUDE.md` があり、他方にはなくても日常業務が回っている。この、困っていないという事実から入る。
- **問いと骨格** : `CLAUDE.md` の役割（セッション開始時に読み込まれる、プロジェクト固有の約束事）、グローバルの `CLAUDE.md` やスキルとの分担、プロジェクトの `CLAUDE.md` が効く場面（一貫した意匠、手動の整合、公開の手順）と、要らない場面を比べる。足すかどうかの基準を示す（同じ指示を繰り返す、ファイル間で手動の整合が要る、同種の誤りが繰り返される）。
- **論点の分担** : 環境の移植（設定、認証、 MCP サーバー、 Auto Memory ）は `claude-code-migration.html` に任せる。この文書は、「何を書くか」「要るか」に絞る。
- **確度の見通し** : 読み込みの仕様は、公式ドキュメントで確かめる。自分の運用の経験は、仕様と分けて書く。

| 主張 | 確度 |
| :--- | :---: |
| プロジェクトの `CLAUDE.md` は、セッション開始時に読み込まれる | 要確認（公式ドキュメントで） |
| `CLAUDE.md` が無くても、グローバルの設定とスキルは使える | 要確認（公式ドキュメントで） |
| 繰り返しの指示や手動の整合が多いほど、プロジェクトの `CLAUDE.md` の効果は大きい | 筆者の経験（一般化しない） |

- **接続（本文で確認済み）** : `claude-code-migration.html` （ 1 章「ユーザーレベル設定」、 3 章「プロジェクトレベル設定」、 5 章「 Auto Memory 」）。
- **接続（論理上の接続）** : `static-site-migration.html` 、 `emdash-learning-guide.html` （公開の手順を持つ文書）、 `suno-mcp-guide.html` （ Claude Code の `claude mcp add` と設定ファイルのスコープを扱う。本文は未通読）。
- **リスク** : 一人称の経験談に寄ると、仕様の説明と区別がつかなくなる。仕様の確認は公式ドキュメントに限り、「 2026 年 11 月時点」のように時点を明記する（ `claude-code-migration.html` と同じ書き方）。

### 6.3 1990 年代の日本での Software AG ・ Adabas ・ Essbase の販売

- **仮題** : 『日本ではどう売られていたのか――Software AG 、 Adabas 、 Essbase の 1990 年代』
- **置き場所** : 3 企業・産業・経済。三本の後に置き、メタ情報帯に「前作」を記す。
- **入口** : 三本が揃って「日本は未確認」と書いている。 `software-ag-overview.html` は「日本は SAGA の担当地域と報じられたが、日本法人との関係は未確認」、 `essbase-history.html` は「富士通と三菱商事の報告書での記載が、日本の販売を指すのかどうか」と、手がかりまで示す。
- **問いと骨格** : 日本法人の有無と設立時期、販売会社、日本語版の初出、導入事例を、年表にまとめる。 `adabas-overview.html` が挙げる Natural の来歴を、周辺として添える。
- **論点の分担** : 年表と製品の概説は、三本に任せる。この文書は、日本に絞る。
- **確度の見通し** : ほぼ全項目が未確認である。文書にする前に事前調査をして、見つかった項目と見つからなかった項目を分ける。

| 主張 | 確度 |
| :--- | :---: |
| 日本は SAGA の担当地域だった | 要確認（報道のみ。 `software-ag-overview.html` ） |
| Hyperion Solutions Japan の設立時期 | 未確認（ `essbase-history.html` ） |
| 日本語版 Essbase の初出は 1990 年代か | 未確認（確認できたのは 2004 年の 7.1 版。 `essbase-history.html` ） |

- **接続（本文で確認済み）** : `adabas-overview.html` （ 8 章）、 `software-ag-overview.html` （ 6 章）、 `essbase-history.html` （ 5 章、 6 章）。
- **資料** : 日本の業界誌、企業の発表資料、有価証券報告書、国立国会図書館の所蔵。取得できる範囲を、事前調査で確かめる。
- **リスク** : 見つからなければ、「見つからなかった」と書くだけの文書になる。その場合は、新しい文書にせず、三本の「確認できていないこと」に、調べた範囲を追記するにとどめる。

---

## 7. 保留中のテーマ

| テーマ | 置き場所の案 | 保留の理由 | 再開の条件 |
| :--- | :--- | :--- | :--- |
| 「民主改革の会」の続報 | 1 日本の政治・制度 | `chudo-kaikaku-rengo-analysis.html` の情報基準日は 2026 年 10 月 13 日で、新党をめぐる状況は流動的である | 新党の動きが、報道で確かめられる形で出たとき |
| Handlebar RC の独立した利用者の声 | 4 FPV ドローンと周辺機器 | 五回の検索で、独立したレビューは見つからなかった（ `handlebar-rc-japan-import.html` ） | 発売後のレビューや実機の報告が、公開されたとき |
| NexRadio 14 と DCS ジンバルの精度・寿命の独立したレビュー | 4 FPV ドローンと周辺機器 | 独立したレビューは見つかっていない（ `nexradio-dcs-gimbal.html` 8 章） | レビューやユーザー報告が、公開されたとき。または、本人が換装して記録できるとき |
| The Zone の物理演算の第三者検証 | 4 FPV ドローンと周辺機器 | 測定による第三者検証が見つからなかった（ `the-zone-fpv-simulator.html` ） | 計測や比較をした資料が、出たとき。または、本人が実機と比べて記録できるとき |

- 前回まで保留していた「中高年を対象にした、社会的比較への向き合い方の研究」は、元の文書（ `superiority-social-comparison.html` ）を廃止したため、保留から外した（別のリポジトリで、統合した新しい文書を作っている）。

---

## 8. 文書を足すときの手順

1. **設計メモを先に作る。** 6 章と同じ項目（仮題、置き場所、入口、問いと骨格、論点の分担、確度の見通し、接続、リスク）を埋めてから、本文に進む。
2. **置き場所を先に決める。** 既存の節に収まるか、節を新設するかを、メモの段階で決める。節の新設は、先にユーザーへ相談する。 `index.html` ・ `megumino.html` ・ `autumn-colors.html` ・ `color-palette.html` の 4 件は、 portal に載せない。
3. **接続先は本文で確かめる。** 題名の印象だけで挙げない。該当する節を特定し、確認できないものは「論理上の接続」と書く。続編は、メタ情報帯に「前作 : …」と書く（ `adabas-overview.html` の例）。本文中のリンクで相互につなぐ場合は、双方向に置く（ `trump-omar-midterms-2026.html` と `us-midterm-2026.html` のように、片方にしかリンクがない状態を避ける）。
4. **統計や書誌は一次資料で確かめる。** 記憶に基づく数字や条文のまま公開しない。確かめられなかった点は、「限界」または「確認できていないこと」の節に、検索した語や取得できなかった理由まで書く。他者の公開した記事に基づく場合は、転載か、要約・再構成かを明示する。
5. **意匠は `contrast-html-style` に従う。** 配色・寸法・マークアップは、スキル（ `~/.claude/skills/contrast-html-style/SKILL.md` ）が正である（ 2026-11-25 に、 `wafu-html-style` から切り替えた）。
6. **`portal.html` と `README.md` を揃える。** カードの追加に加え、「収録 N 点」、 `Updated:` の日付、 `nav.toc` の数字、 `README.md` の総本数と節の表を更新する（ `CLAUDE.md` の「件数が載る場所」）。カードは、同じ話題の隣に入れる（末尾に積まない）。カードの説明文に基準日を書いた文書（ `ai-industry-comparison.html` など）を更新したときは、その基準日も合わせる。
7. **この文書を更新する。** 1 章の表（本数・平均字数）、 3 章の宿題、 5 章の順位を書き直す。閉じた宿題は 3 章から、書き終えた候補は 5 章と 6 章から削除する。 `CLAUDE.md` の冒頭にある文書数も、実際の本数に合わせる。
