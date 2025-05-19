# Slack Thread Bot – Fork Edition

> **Forked by Kenichi Nakachi**  
> Original author & repo: [solaoi/dify-plugin-slack-thread-bot](https://github.com/solaoi/dify-plugin-slack-thread-bot)

このリポジトリは、Slack Thread Bot プラグインを個人的な用途に合わせて
改変・拡張した **フォーク版** です。  
オリジナルからの主な変更点は次のとおりです。

| 変更点 | 概要 |
|--------|------|
| **DM 対応** | `message.im` をハンドリングし、メンション不要で 1 : 1 DM に応答 |
| **manifest 更新** | `name`・`label` に “-fork” を追加し、著者欄に自分の名前を明記 |
| **日本語 README の簡素化** | オリジナル README を削除し、フォークで追加した部分のみ記載 |

## インストール

1. GitHub から **このフォーク** を指定して Dify にプラグインをインストール  
https://github.com/<YOUR_ACCOUNT>/slack-thread-bot-fork

2. Slack 側で App を作成し、以下のスコープとイベントを設定  
Scopes: app_mentions:read, channels:history, im:history, chat:write, files:read
Events: app_mention, message.channels, message.im

3. Dify で **Bot Token と接続先 App** を設定して完了。

## ライセンス

元リポジトリと同じ **MIT License** を継承しています。  
フォーク部分の変更・再配布も MIT ライセンスに従って自由に行えます。