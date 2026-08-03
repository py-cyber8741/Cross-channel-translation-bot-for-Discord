# Cross-channel-translation-bot-for-Discord
Cross-channel translation bot for Discord

https://github.com/py-cyber8741/Cross-channel-translation-bot-for-Discord/releases/download/1.1.1/transbot.exe

DiscordのBOTトークンは必須ですが、geminiは任意なので必須ではありません。


取扱説明書
本アプリケーションは、Discordサーバー間やチャンネル間で多言語のリアルタイム翻訳を行う高機能ツールです。GUIによる直感的な管理、DM対応、画像ビューワー、AI連携など、多彩な機能を備えています。


🤖 TransBot 取扱説明書


1. 初期設定とBotの起動
アプリケーションを起動したら、まずはDiscord Botと連携するための設定を行います。

設定画面を開く: 画面右上の「⚙️ 設定」ボタンをクリックします。

Tokenの入力: 「基本設定」タブの「Bot Token:」に、Discord Developer Portalで取得したBotのトークンを入力します。

Gemini API Key (任意): AIによる翻訳・推敲機能を使用する場合は入力します。

UI言語の変更: 画面の言語を日本語や英語などに切り替えられます。

保存と起動: 「保存」を押してメイン画面に戻り、「Bot起動」ボタンを押すとBotがオンラインになります。


3. メイン画面の基本操作
メイン画面は、新着翻訳フィード、チャンネル設定、システムログの3つのエリアで構成されています。枠の境界線をマウスでドラッグすることで、各エリアのサイズを自由に調整できます。画面右上の「A+」「A-」ボタンで文字サイズの拡大・縮小も可能です。

翻訳グループの作成と管理

サーバー内のチャンネルを「グループ」としてまとめることで、そのグループ内のチャンネル同士で相互に翻訳が送信されるようになります。

チャンネル取得: 画面中央の「📡 チャンネル取得」ボタンを押すと、右側にBotが参加しているサーバーとチャンネルのリスト（サイドバー）が表示されます。

情報の入力: サイドバーのチャンネルをダブルクリックすると、GID (サーバーID) と ChID (チャンネルID) が自動入力されます。

言語の指定: 「🌐 言語一覧」から翻訳先の言語をダブルクリックして Lan に入力します。

グループ名: 任意のグループ名（例: Group-1）を Grp に入力します。

追加/更新: 「追加/更新」ボタンを押すと階層ツリーに登録されます。

その他のメイン画面機能

Webhook機能: チェックを入れると、Botがユーザーのアイコンと名前を模倣して翻訳を送信します（Discord側で見やすくなります）。

国旗スタンプ翻訳: チェックを入れると、Discord上でメッセージに国旗のリアクション（例: 🇺🇸）を付けた際、Botがその言語に翻訳して返信します。

新着翻訳フィード: 稼働中の全サーバーで行われた翻訳がリアルタイムに流れます。リストをダブルクリック（または右クリック）すると、対象チャンネルの「ログビューワー」が開きます。


5. 各種ツールウィンドウ
6. 
階層ツリーのチャンネルや、新着フィードからアクセスできる強力な管理ツールです。すべてのウィンドウで枠のドラッグサイズ調整に対応しています。

📜 ログビューワー

対象チャンネルの過去のメッセージを閲覧し、操作できます。

翻訳表示: 「🌐 Translate」ボタンで、過去のログを指定した言語に一括翻訳して表示します。

画像ビューワー機能: ログ内の画像（🔍マーク）をクリックすると原寸大で開きます。

マウスホイール: 画像の拡大・縮小（ズーム）。

左クリック＋ドラッグ: 拡大した画像を掴んで自由に移動（パン操作）。

右クリック: 画像の保存。

クイック返信: ログを見ながら、画面下部からメッセージを送信できます。

直近のBot発言を削除: 誤って送信したBotのメッセージをワンクリックで削除します。


💬 BOT発言ウィンドウ

ツリー上でチャンネルを右クリックし、「💬 このチャンネルに発言」を選ぶと開きます。

送信モード: 「そのまま送信」「翻訳して送信」「AIで翻訳/推敲」から選択できます。

AI翻訳: Gemini APIを利用し、指定した言語のより自然な文章に推敲・翻訳して送信します。

リアルタイムログ: 上部にそのチャンネルの最新の会話状況がリアルタイムで流れます。


✉️ DM (ダイレクトメッセージ) 管理

メイン画面右上の「✉️ DM」ボタンから開きます。Bot宛てに届いたDMの確認と返信が可能です。

履歴の同期: 「🔄 過去のDMをDiscordから同期」を押すと、Botが過去にやり取りしたユーザー履歴を復元します。

ユーザー詳細情報: 左側のユーザーリストを右クリック ＞「ℹ️ ユーザー情報を表示」で、そのユーザーのID、保存済みDM数などの詳細情報をテキストで表示・一括コピーできます。

翻訳返信: DMに対しても、指定言語に翻訳した上で返信が可能です。

🌐 多言語チャンネル自動生成 (Auto Clone)

サイドバーの「📡 チャンネル取得」で表示されたツリー上のチャンネルを右クリックし、「🌐 多言語チャンネルを自動生成」を選びます。

元となるチャンネルを複製し、選択した複数の言語（例: 英語、韓国語、中国語）専用のチャンネルを一気に自動作成します。

作成されたチャンネルは、自動的に翻訳グループに登録・相互接続されます。


5. スパム対策・BAN設定 (システム管理)
6. 
設定画面から、荒らしや迷惑行為への対策を設定できます。

スパム判定: 「スパム判定枠（分）」と「判定回数」を設定します。制限を超えて連続投稿したユーザーは自動的に「一時停止（Suspend）」となり、翻訳がストップします。

BAN設定: 特定のユーザーIDやサーバーIDを登録することで、Botがその対象からのメッセージを完全に無視するようになります。


8. Discord側 スラッシュコマンド
9. 
サーバーの管理者やユーザーがDiscordのチャット欄から直接実行できるコマンドです。


コマンド,説明,権限

/chset,現在のサーバーで指定した数のチャンネルをグループ化し、相互翻訳を設定します。,管理者

/chdel,チャンネルの翻訳グループ登録を解除・削除します。,管理者

/setup,設定のON/OFFや言語変更がボタンで瞬時に行えるコントロールパネルを表示します。,管理者

/chadd,既存の翻訳グループに新しいチャンネルを追加します。,管理者

/chmode,Webhookモードと国旗リアクション翻訳のON/OFFを切り替えます。,管理者

/ai,入力したテキストをAI（Gemini）で翻訳・推敲して送信します。,全員

/botconfig status,現在のBotのスパム判定基準やBAN人数などのステータスを確認します。,システム管理者

/botconfig spam,スパム（連投）判定の時間と回数を設定します。,システム管理者

/botconfig notify,新着翻訳フィード通知のON/OFFおよび言語を設定します。,システム管理者

/botconfig ban,指定したユーザーをBANリストに追加します。,システム管理者

/botconfig unban,指定したユーザーのBANや一時停止を解除します。,システム管理者




Cross-channel translation bot for Discord

https://github.com/py-cyber8741/Cross-channel-translation-bot-for-Discord/releases/download/1.1.1/transbot.exe

A Discord BOT token is required, but a Gemini API key is optional and not mandatory.

User Manual

This application is a highly functional tool that performs multilingual real-time translation between Discord servers and channels. It comes equipped with a variety of features, including intuitive GUI-based management, DM support, an image viewer, and AI integration.

🤖 TransBot User Manual

Initial Setup and Bot Startup

After launching the application, you must first configure the settings to link it with your Discord Bot.

Open Settings Screen: Click the "⚙️ Settings" button in the upper right corner of the screen.

Enter Token: In the "Basic Settings" tab, enter the Bot token obtained from the Discord Developer Portal into the "Bot Token:" field.

Gemini API Key (Optional): Enter this if you plan to use the AI-powered translation and text refinement features.

Change UI Language: You can switch the application's interface language (e.g., between Japanese and English).

Save and Start: Click "Save" to return to the main screen, then click the "Start Bot" button to bring the Bot online.

Basic Operations on the Main Screen

The main screen consists of three areas: the New Translation Feed, Channel Settings, and System Log. You can freely adjust the size of each area by dragging the borders with your mouse. 

You can also enlarge or reduce the text size using the "A+" and "A-" buttons in the upper right corner.

Creating and Managing Translation Groups

By bundling channels within a server into a "Group," translations will automatically be sent back and forth between those channels.

Fetch Channels: Clicking the "📡 Fetch Channels" button in the center of the screen will display a list (sidebar) on the right showing the servers and channels the Bot has joined.

Input Information: Double-clicking a channel in the sidebar will automatically input its GID (Server ID) and ChID (Channel ID).

Specify Language: Double-click the target translation language from the "🌐 Language List" to input it into the "Lan" field.

Group Name: Enter a desired group name (e.g., Group-1) into the "Grp" field.

Add/Update: Click the "Add/Update" button to register it in the hierarchical tree.

Other Main Screen Features

Webhook Feature: When checked, the Bot will impersonate the user's icon and name when sending translations (making it much easier to read on Discord).

National Flag Reaction Translation: When checked, if a user reacts to a message on Discord with a national flag emoji (e.g., 🇺🇸), the Bot will translate the message into that language and reply.

New Translation Feed: Translations occurring across all active servers will flow here in real-time. Double-clicking (or right-clicking) an item in the list will open the "Log Viewer" for that specific channel.

Various Tool Windows

These are powerful management tools accessible from the hierarchical tree channels or the new translation feed.

All windows support size adjustment by dragging the borders.


📜 Log Viewer

View and manage past messages of a target channel.

Display Translation: Use the "🌐 Translate" button to batch-translate past logs into a specified language and display them.

Image Viewer Feature: Clicking an image (🔍 icon) in the log opens it in its original size.

Mouse Wheel: Zoom in/out of the image.

Left Click + Drag: Grab and freely move the enlarged image (pan).

Right Click: Save the image.

Quick Reply: You can send messages from the bottom of the screen while looking at the logs.

Delete Recent Bot Messages: Delete a mistakenly sent Bot message with a single click.


💬 BOT Speech Window

Opens when you right-click a channel on the tree and select "💬 Speak in this channel".

Transmission Mode: Choose from "Send as is," "Translate and send," or "AI translate/refine."

AI Translation: Utilizes the Gemini API to refine and translate your text into more natural phrasing in the specified language before sending.

Real-time Log: The latest conversation activity for that channel streams in real-time at the top of the window.


✉️ DM (Direct Message) Management

Open this from the "✉️ DM" button in the upper right of the main screen. You can check and reply to DMs sent directly to the Bot.

Sync History: Clicking "🔄 Sync past DMs from Discord" restores the history of users the Bot has interacted with previously.

User Details: Right-click the user list on the left > "ℹ️ Show User Info" to display and easily copy detailed information as text, such as the user's ID and the number of saved DMs.

Translated Reply: You can translate your replies to DMs into a specified language before sending.


🌐 Automatic Multilingual Channel Generation (Auto Clone)

Right-click a channel on the tree displayed by "📡 Fetch Channels" and select "🌐 Auto-generate multilingual channels".
This duplicates the base channel and instantly creates dedicated channels for multiple selected languages (e.g., English, Korean, Chinese). 

The created channels are automatically registered into a translation group and interconnected.

Anti-Spam & BAN Settings (System Management)
You can configure countermeasures against trolls and disruptive behavior from the settings screen.

Spam Detection: Set the "Spam Detection Timeframe (minutes)" and "Detection Count". Users who consecutively post beyond this limit will automatically be put into "Suspend" status, and their translations will stop.

BAN Settings: By registering specific user IDs or server IDs, the Bot will completely ignore any messages from those targets.

Discord Slash Commands

These are commands that server administrators and users can execute directly from the Discord chat input.



Command,Description,Permission

/chset,Groups a specified number of channels in the current server and sets up mutual translation.,Administrator

/chdel,Unregisters and deletes a channel from a translation group.,Administrator

/setup,Displays a control panel where settings (ON/OFF) and languages can be changed instantly via buttons.,Administrator

/chadd,Adds a new channel to an existing translation group.,Administrator

/chmode,Toggles Webhook mode and national flag reaction translation ON/OFF.,Administrator

/ai,Translates and refines the inputted text using AI (Gemini) before sending.,Everyone

/botconfig status,"Checks the current Bot status, such as spam detection criteria and the number of banned users.",System Admin

/botconfig spam,Sets the timeframe and count threshold for spam (continuous posting) detection.,System Admin

/botconfig notify,Toggles the new translation feed notification ON/OFF and sets its language.,System Admin

/botconfig ban,Adds a specified user to the BAN list.,System Admin

/botconfig unban,Lifts a BAN or suspension for a specified user.,System Admin
