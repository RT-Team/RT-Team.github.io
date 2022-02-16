[Back to notes](/notes)
* * *
# How to user RT embed command
It is possible to make an embedding by doing the following.
```
rt!embed [url or webhook] "color code" title
content
```
If you set the part of `[url or webhook]` to `url`, you can create a URL where the embedded will appear when you send it.
If you set it to `webhook`, you can send an embedded with a webhook.  
In the case of `url`, it may not be reflected immediately. Let's wait. And there will be no newlines.  
In this case, you don't need to include the URL, but you won't be able to edit the message.  
The color code is embedded color, and please see [here] (https://rt-team.github.io/en/notes/color) for how to specify it.。  
In the case of web hooks, you can write the contents with markdown.  
So it is possible to write as follows.
```
rt!embed webhook "color code" title
description
## field
field description
## field
field description
## !Fields that don't line up sideways
Description of the field
## !Fields that don't line up sideways
Description of the field
### Fields in the field
※You can't make a deeper field.
```
※`#`一つだけは使えません、`## `か`## !`または`### `が使えます。  
また横に並ばないフィールドというのは、そのフィールドの項目が前のフィールドの右に来ることがないということです。  
右にくることがあるのはWeb版とPC版のDiscordのみで、iOSやiPad OSそしてAndroidなどでは普通のフィールドと変わりがないです。  
それと普通マークダウンでは改行をする際にスペースを二つ置く必要がありますがこれはする必要はないです。

## メモ
デフォルトでは作られる埋め込みの投稿者は実行者の名前になりアイコンも実行者のアイコンになります。  
これはWebhookを使用して送っているからで、もしRTの名前とアイコンで埋め込みを投稿して欲しい場合は`--rticon`をタイトルの前に入れてください。  
それと`rt>embed`をチャンネルのトピックに入れることで、そのチャンネルに送ったメッセージを自動でEmbedにしてくれます。  
また既に作ったものに返信をしてコマンドを実行すれば編集ができます。

## 例
### 普通
```
rt!embed url null ようこそ
まずは#ルールでルールを確認しましょう。
```
### 処罰履歴
```
rt!embed webhook red 処罰履歴
@tasurenをKickしました。
## 理由
えっちなことを言ったから。
```
### ルール
```
rt!embed webhook ルール
## !ルール 一
仲良く
## !ルール 二
NSFWなものはNG
```
