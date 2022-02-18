[戻る｜Back](/)
* * *

English explanation is at the bottom.

# りつたんの使い方
りつたんとは[Discordの便利なBotのRT](https://rt-bot.com)の音楽再生と読み上げだけを使えるようにしたRTのサブBotです。  
りつたんを使えばRTの読み上げと音楽再生を同時利用できます。  
プリフィックスは`rt#`でスラッシュコマンドに対応しています。  
[招待リンク](https://discord.com/api/oauth2/authorize?client_id=888635684552863774&permissions=172339022401&scope=bot%20applications.commands) ｜ [サポートサーバー](https://discord.gg/ugMGw5w)

## 目次
* [一般コマンド](#一般コマンド)
* [音楽プレイヤー](#音楽プレイヤー)
* [読み上げ](#読み上げ)
* [クレジット](#クレジット)

### 一般コマンド
`rt#help`または`rt#info`でこのサイトのURLを表示します。

### 音楽プレイヤー
YouTube,ニコニコ動画そしてSoundCloudの再生に対応しています。  
スキップコマンドなどの一部のコマンドは他に音楽を聴いている人がいる場合DJロールまたは管理者権限がないと実行できません。  
※DJロールについては下に説明があります。
#### rt#play URL
渡されたURLの音楽を再生します。  
上で書いた通りYouTubeとニコニコ動画そしてSoundCloudに対応しています。  
もし渡されたのがURLじゃない場合はYouTubeで検索を行います。  
またYouTubeの再生リストのURLが渡された場合はそのプレイリストにある曲を全てキューに追加します。  
※キューは再生予定の音楽リストのことです。
#### rt#queue
キューにある曲を表示します。  
またキューにある曲を選択してキューから削除することもできます。  
もしプレイリストを作っている場合はキューにある曲を選択してプレイリストに曲を追加することもできます。
#### rt#clear
キューにある曲を全て消します。
#### rt#skip
現在再生してる曲を停止して次の曲を再生します。
#### rt#pause
現在再生している曲を一時停止します。  
もし既に一時停止している場合は再生再開します。  
注意：再生停止状態で放置するとりつたんは嫌な気分になって音楽再生を終了します。
#### rt#loop
現在再生している曲をループ再生します。  
もし既にループ再生している場合はループ再生を解除します。
#### rt#shuffle
キューにある曲をシャッフルします。
#### rt#now
現在再生している曲の情報を表示します。
#### rt#playlist
プレイリスト機能です。
##### rt#playlist show
プレイリストにある曲を表示します。  
また表示されたプレイリストにある曲を選択して削除することもできます。
##### rt#playlist create 名前
`名前`という名前でプレイリストを新たに作成します。  
十個まで作成可能です。
##### rt#playlist delete 名前
`名前`という名前のプレイリストを削除します。
##### rt#playlist add URL
`URL`の音楽をプレイリストに追加します。  
一つのプレイリストに800曲まで追加できます。
##### rt#playlist play
プレイリストにある曲から再生をします。
#### rt#disconnect
音楽再生を終了します。

### 読み上げ
テキストチャンネルに送信されたメッセージの内容をボイスチャンネルで再生をします。
#### rt#tts join
読み上げを開始します。
#### rt#tts leave
読み上げを終了します。
#### rt#tts voice
読み上げに使う声を変更します。  
ゆっくり霊夢やゆっくり魔理沙など使えます。  
注意：初音ミクがありますが安定してないです。リアル消失になりかねないので注意。
#### rt#tts dictionary
辞書機能で指定した言葉は別の言葉に交換します。  
`rt#tts dictionary`と実行すると辞書のリストが表示されます。
エイリアス：`dic`, `辞書`
##### rt#tts dictionary set 交換対象 交換先
辞書を追加します。  
実行すると読み上げ時に`交換対象`が`交換先`に交換されます。
##### rt#tts dictionary delete 交換対象
辞書から`交換対象`を削除します。
#### rt#tts routine
ネタ音声機能です。  
指定した言葉が送信された場合は指定した音声ファイルを再生します。  
りつたんを汚したくはないですが`そうだよ`を送信した際に[そうだよ](https://rt-bot.com/tts/routine/634763612535390209-MUR.wav)の音声ファイルを再生するようにしたりできます。  
このネタ音声登録はりつたんからはできないので[RT](https://rt-bot.com)から登録してください。

### クレジット
りつたんのアイコンの絵は[真夜月。さん](https://coconala.com/users/246022)に作ってもらいました！  
ありがとうございます。

# How to use Ritsu-tan
Ritsu-tan is a sub-bot of [Discord's useful bot RT](https://rt-bot.com) that allows you to use only music playback and reading.  
With Ritsu-tan, you can use RT reading and music playback at the same time.  
The prefix is `rt#` and it supports slash commands.  
[招待リンク](https://discord.com/api/oauth2/authorize?client_id=888635684552863774&permissions=172339022401&scope=bot%20applications.commands) ｜ [サポートサーバー](https://discord.gg/ugMGw5w)

## Table of Contents
* [General commands](#General commands)
* [Music Player](#Music Player)
* [Readout](#Readout)
* [Credit](#Credit)

### General Commands.
`rt#help` or `rt#info` will show the URL of this site.

### Music Player
Supports playback of YouTube, Nico Nico Douga and SoundCloud.  
Some commands, such as the skip command, cannot be executed if there are other people listening to the music and you do not have a DJ role or administrator privileges.  
For more information on DJ roles, see below.
#### rt#play URL
This will play the music from the URL given to you.  
As mentioned above, it supports YouTube, Nico Nico Douga, and SoundCloud.  
If the URL is not the one given, it will search YouTube.  
If the URL is not a URL, it will search YouTube. If the URL is a YouTube playlist, it will add all the songs in the playlist to the queue.  
A queue is a list of music to be played.
#### rt#queue
Displays the songs in the queue.  
You can also select a song in the queue to remove it from the queue.  
If you have created a playlist, you can also select a song in the queue to add it to the playlist.
#### rt#clear
Clear all songs in the queue.
#### rt#skip
Stop the currently playing song and play the next song.
#### rt#pause
Pause the currently playing song.  
If the song is already paused, it will resume playing.  
Note: If you leave the music playing while it is paused, Rintan will feel uncomfortable and quit playing music.
#### rt#loop
Loop the currently playing song.  
If it is already looping, it will cancel the loop.
#### rt#shuffle
Shuffle the songs in the queue.
#### rt#now
Displays information about the currently playing song.
#### rt#playlist
Playlist function.
##### rt#playlist show
Shows the songs in the playlist.  
You can also select a song in the displayed playlist to delete it.
##### rt#playlist create name
Creates a new playlist with the name `name`.  
Up to ten playlists can be created.
##### rt#playlist delete name
Delete a playlist with the name `name`.
##### rt#playlist add URL
Add the music of `URL` to the playlist.  
Up to 800 songs can be added to one playlist.
##### rt#playlist play
Play a song from the playlist.
#### rt#disconnect
Ends music playback.

### readout
Play back the content of a message sent to the text channel on the voice channel.
#### rt#tts join
Starts reading out loud.
#### rt#tts leave
End reading.
#### rt#tts voice
Change the voice used for reading out loud.  
You can use Slowly Reimu, Slowly Marisa, etc.  
Note: Hatsune Miku is available, but it's not stable. Be careful, it may cause real loss.

### Credits
The picture of Ritsu-tan's icon is by [Mayatsuki](https://coconala.com/users/246022) for making the picture of Ritsu-tan!  
Thank you very much.  
Translated with www.DeepL.com/Translator (free version)