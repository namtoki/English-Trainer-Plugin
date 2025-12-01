# /words コマンド

引数: $ARGUMENTS

## 処理フロー

### 1. words/ ディレクトリ配下の全ファイルを読み込み

以下のファイルを全て Read してください:
- `words/02_verb/*.md`
- `words/03_adjective_noun/*.md`
- `words/04_adverb/*.md`
- `words/cliche.md`
- `words/framework.md`

### 2. 引数に応じた処理

#### `$ARGUMENTS` が数字のみの場合

1. 指定された数だけ、以下のリスト (優先度順) から英単語をピックアップしてください。ただし、既に `words/` にリストされている単語は除外すること。
   - NGSL (New General Service List) - 約2,800語で一般英文の約92%をカバー
   - GSL (General Service List) - Michael Westが1953年に作成した古典的リスト約2,000語
   - AWL (Academic Word List) - 学術論文・教科書によく出る570語族
   - COCA頻度リスト - Corpus of Contemporary American Englishに基づく頻度順リスト
   - SVL 12000 (Standard Vocabulary List)

2. ピックアップした単語を適切なファイルに追加してください。

#### `$ARGUMENTS` が具体的な英単語の場合

1. その単語が既に `words/` に存在するか確認
2. 存在する場合: その行をコンソールに表示するのみ
3. 存在しない場合: 適切なファイルに追加

### 3. 書き込みフォーマット

H2 セクションで分類し、各行に以下の情報を記載:
```md
## Sound Action
- `shout` /ʃaʊt/                    ([Neutral] 叫ぶ、大声で言う)    He shouted across the street.
  - `yell` /jel/                    ([Casual] 叫ぶ、怒鳴る)         The coach yelled at the players.
  - `scream` /skriːm/               ([Neutral] 叫ぶ、悲鳴を上げる)  He screamed for help.
```

### 4. 書き込み先ファイル一覧

動詞:
- `words/02_verb/0_AUX.md` - 助動詞のような働きの動詞
- `words/02_verb/1_SVC.md` - SVC 文型の動詞
- `words/02_verb/2_SVOC.md` - SVOC 文型の動詞
- `words/02_verb/3_SVOO.md` - SVOO 文型の動詞
- `words/02_verb/4_Opinion.md` - 考えを述べる際に使用する表現 (SV, SVO)
- `words/02_verb/5_Cognitive.md` - 認識を説明する時に使用する表現 (SV, SVO)
- `words/02_verb/6_Task.md` - タスク管理関連の表現 (SV, SVO)
- `words/02_verb/7_Description.md` - 何かを説明する時に使える表現 (SV, SVO)
- `words/02_verb/8_Common.md` - その他の表現 (SV, SVO)

形容詞・名詞:
- `words/03_adjective_noun/0_Hedge.md` - ぼやけさせる名詞、形容詞
- `words/03_adjective_noun/1_Business.md` - 仕事でよく使う名詞、形容詞
- `words/03_adjective_noun/2_Politics_Religion.md` - 政治、宗教関連
- `words/03_adjective_noun/3_Law_Crime.md` - 法律、犯罪関連
- `words/03_adjective_noun/4_Education.md` - 教育、学術関連
- `words/03_adjective_noun/5_Science.md` - 科学関連
- `words/03_adjective_noun/6_Community.md` - 金融、不動産などの公共関連
- `words/03_adjective_noun/7_Health.md` - 病院、健康、医療関連
- `words/03_adjective_noun/8_Life.md` - 日常関連
- `words/03_adjective_noun/9_Assessment.md` - 客観的な評価を表現する名詞、形容詞

副詞:
- `words/04_adverb/0_Conjunction.md` - 接続副詞
- `words/04_adverb/1_Reason.md` - 理由、目的の副詞
- `words/04_adverb/2_How.md` - 「どのように」を説明する副詞
- `words/04_adverb/3_Condition.md` - 条件を表す副詞
- `words/04_adverb/4_Concession.md` - 譲歩を表す副詞
- `words/04_adverb/5_Feeling.md` - 主観による情報を補足する副詞
- `words/04_adverb/6_When_Where.md` - 時間、場所を補足する副詞

### 5. YouGlish で実例動画を検索 (共通処理)

追加した単語/表現について、YouGlish のリンクをコンソールに出力してください:
- URL形式: `https://youglish.com/pronounce/{単語}/english`
- WebFetch で該当ページにアクセスし、動画IDとタイムスタンプを取得
- 取得した動画を YouTube URL 形式で出力

例:
```
YouTube Videos for "shout":
- YouGlish: https://youglish.com/pronounce/shout/english

1. https://youtube.com/watch?v=xxxxx&t=120 (2:00)
2. https://youtube.com/watch?v=yyyyy&t=45 (0:45)
...
```
