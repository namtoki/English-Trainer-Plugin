# /cliche コマンド

引数: $ARGUMENTS

## 処理フロー

### 1. 既存データの読み込み

`words/cliche.md` を Read してください。

### 2. 引数に応じた処理

#### `$ARGUMENTS` が数字のみの場合

1. 指定された数だけ、重要な定型表現をピックアップしてください。ただし、既に `words/cliche.md` にリストされている表現は除外すること。
2. ピックアップする定型表現の例:
   - 挨拶: Good morning., How are you?, Nice to meet you.
   - 感謝: Thank you so much., I really appreciate it.
   - 謝罪: I'm sorry., My apologies., Excuse me.
   - 依頼: Could you please...?, Would you mind...?
   - 同意: I agree., That's right., Exactly.
   - 相槌: I see., Really?, That's interesting.
   - 確認: Is that correct?, Am I right?
   - 提案: How about...?, Why don't we...?
   - その他ビジネスや日常で頻出する定型表現

3. `words/cliche.md` に追加

#### `$ARGUMENTS` が具体的な定型表現の場合

1. その表現が既に `words/cliche.md` に存在するか確認
2. 存在する場合: その行をコンソールに表示するのみ
3. 存在しない場合: `words/cliche.md` に追加

### 3. 書き込みフォーマット

H2 セクションで分類し、各行に以下の情報を記載:
```md
## Greetings
- `Good morning.`                   ([Formal] おはようございます)     Good morning, everyone.
- `How's it going?`                 ([Casual] 調子どう?)              Hey, how's it going?
- `Nice to meet you.`               ([Neutral] はじめまして)          Nice to meet you, Mr. Smith.

## Gratitude
- `Thank you so much.`              ([Neutral] 本当にありがとう)       Thank you so much for your help.
- `I really appreciate it.`         ([Formal] 本当に感謝します)        I really appreciate your support.
```

### 4. YouTube動画検索 (共通処理)

MCP サーバー `youtube` を使用して、追加した表現が使用されている動画を検索してください:
- 再生回数が多い動画を10件ピックアップ
- 各動画について、その表現が使われている再生時間も特定
- URL とタイムスタンプをコンソールに出力

例:
```
YouTube Videos for "I really appreciate it":
1. [Title] - https://youtube.com/watch?v=xxx&t=120 (2:00)
2. [Title] - https://youtube.com/watch?v=yyy&t=45 (0:45)
...
```
