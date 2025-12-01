# 単語・表現の書き込みフォーマット

このスキルは、words/ ディレクトリへの単語・表現の追加時に使用するフォーマットを定義します。

---

## 共通フォーマット

H2 セクションで分類し、各行に以下の情報を記載:

```md
- `単語/表現` /発音記号/ ([Register] 日本語訳) 例文
  - `類義語` /発音記号/ ([Register] 日本語訳) 例文
```

### Register (使用場面)

- `[Formal]` - フォーマル・ビジネス
- `[Neutral]` - 一般的
- `[Casual]` - カジュアル・口語

---

## 動詞の例 (words/02_verb/)

```md
## Sound Action
- `shout` /ʃaʊt/                    ([Neutral] 叫ぶ、大声で言う)    He shouted across the street.
  - `yell` /jel/                    ([Casual] 叫ぶ、怒鳴る)         The coach yelled at the players.
  - `scream` /skriːm/               ([Neutral] 叫ぶ、悲鳴を上げる)  He screamed for help.
```

---

## 定型表現の例 (words/cliche.md)

```md
## Greetings
- `Good morning.`                   ([Formal] おはようございます)     Good morning, everyone.
- `How's it going?`                 ([Casual] 調子どう?)              Hey, how's it going?
- `Nice to meet you.`               ([Neutral] はじめまして)          Nice to meet you, Mr. Smith.

## Gratitude
- `Thank you so much.`              ([Neutral] 本当にありがとう)       Thank you so much for your help.
- `I really appreciate it.`         ([Formal] 本当に感謝します)        I really appreciate your support.
```

---

## フレームワーク表現の例 (words/framework.md)

```md
## Reason & Explanation
- `S V in the sense that S V`       ([Formal] SがVするという意味で)   It's correct in the sense that it follows the rules.
- `The reason why S V is that S V`  ([Neutral] SがVする理由は...)      The reason why I'm late is that I missed the train.

## Contrast
- `On the one hand S V, on the other hand S V`  ([Formal] 一方では...他方では)  On the one hand it's expensive, on the other hand it's high quality.
- `While S V, S V`                  ([Neutral] ...する一方で)          While I agree with the idea, I have some concerns.

## Addition
- `In addition to N, S V`           ([Formal] Nに加えて)               In addition to English, she speaks French.
- `Not only S V but also S V`       ([Neutral] ...だけでなく...も)      Not only did he apologize but also offered compensation.
```

---

## 書き込み先ファイル一覧

### 動詞 (words/02_verb/)
- `0_AUX.md` - 助動詞のような働きの動詞
- `1_SVC.md` - SVC 文型の動詞
- `2_SVOC.md` - SVOC 文型の動詞
- `3_SVOO.md` - SVOO 文型の動詞
- `4_Opinion.md` - 考えを述べる際に使用する表現
- `5_Cognitive.md` - 認識を説明する時に使用する表現
- `6_Task.md` - タスク管理関連の表現
- `7_Description.md` - 何かを説明する時に使える表現
- `8_Common.md` - その他の表現

### 形容詞・名詞 (words/03_adjective_noun/)
- `0_Hedge.md` - ぼやけさせる名詞、形容詞
- `1_Business.md` - 仕事でよく使う名詞、形容詞
- `2_Politics_Religion.md` - 政治、宗教関連
- `3_Law_Crime.md` - 法律、犯罪関連
- `4_Education.md` - 教育、学術関連
- `5_Science.md` - 科学関連
- `6_Community.md` - 金融、不動産などの公共関連
- `7_Health.md` - 病院、健康、医療関連
- `8_Life.md` - 日常関連
- `9_Assessment.md` - 客観的な評価を表現する名詞、形容詞

### 副詞 (words/04_adverb/)
- `0_Conjunction.md` - 接続副詞
- `1_Reason.md` - 理由、目的の副詞
- `2_How.md` - 「どのように」を説明する副詞
- `3_Condition.md` - 条件を表す副詞
- `4_Concession.md` - 譲歩を表す副詞
- `5_Feeling.md` - 主観による情報を補足する副詞
- `6_When_Where.md` - 時間、場所を補足する副詞

### その他 (words/01_framework/)
- `cliche.md` - 定型表現
- `framework.md` - 構文パターン
