---
title: 変更履歴
---

### 2025/01/29 2.16.46-jp-1

#### 全般

- 不具合修正: Al+F4キーで WinMerge が終了せずにツールメニューが表示される問題を修正した。（[#2592](https://github.com/WinMerge/winmerge/issues/2592)）。  
- 不具合修正: Windowsのアニメーション効果が有効な状態でWinMergeを最大化して起動すると、一瞬タイトルバーの描画位置がずれる問題を修正した。

#### フォルダー比較

- 不具合修正: 左右のファイル名の大文字小文字も異なる場合、片方のファイルを削除後残ったファイルを反対側にコピーするとファイル名の大文字小文字が一致しない問題を修正した。（[#2599](https://github.com/WinMerge/winmerge/issues/2599)）。  
- フォルダー比較ウインドウで左側から右側または逆方向にコピーする際、選択された項目に同一ファイルやスキップされたファイルが含まれていた場合に差異のあるファイルのみをコピーするか確認するダイアログを表示するようにした。（[PR #2622](https://github.com/WinMerge/winmerge/pull/2622)）。

#### プラグイン

- 不具合修正: バージョン2.16.43以降、プラグイン -> 比較前処理プラグイン メニューが正しく表示されない問題を修正した。  
- 不具合修正: PowerPoint ファイルを CompareMSPowerPointFiles.sct プラグインで比較するとエラー 0x80048010 が発生することがある問題を修正した。
- ファイル番号を指定してプラグインを適用できる機能を追加した。（[PR #2598](https://github.com/WinMerge/winmerge/pull/2598)）。  
- プラグインウィンドウをリサイズ可能にした。プラグインの種類ごとに表示するようにした。（[PR #2621](https://github.com/WinMerge/winmerge/pull/2621)）。

#### マニュアル

- 不具合修正: WinMergeマニュアル内の誤字を修正した（[#2597](https://github.com/WinMerge/winmerge/issues/2597)）

### 2024/12/29 2.16.44-jp-4

#### 全般

- 不具合修正: メニューが非表示の場合、Shift+Altキーで言語を切り替えると、メニューにフォーカスが当たってしまう問題を修正した。
  ([PR #2572](https://github.com/WinMerge/winmerge/pull/2572))(PRをいただきました。ありがとうございます。)
- オプションダイアログの[比較/一般]カテゴリに[ファイル末尾の改行文字の有無を無視する」オプションを追加した。
  ([PR #2573](https://github.com/WinMerge/winmerge/pull/2573), [#203](https://github.com/WinMerge/winmerge/issues/203), [#989](https://github.com/WinMerge/winmerge/issues/989), [#2317](https://github.com/WinMerge/winmerge/issues/2317))

#### ファイル比較

- 不具合修正: ロケーションペイン内の移動ブロックをつなぐ線の高さが正しくない場合がある問題を修正した。
  ([#2543](https://github.com/WinMerge/winmerge/issues/2543))

#### フォルダー比較

- 不具合修正: フォルダー比較が完了する前にフォルダーアイコンに緑のチェックマークが付く問題を修正した。  
  ([#2562](https://github.com/WinMerge/winmerge/issues/2562))

#### プラグイン

- 不具合修正: CompareMSWordFiles プラグイン: RTFファイルを比較すると変換確認ウインドウが表示される問題を修正した。 
  ([#2566](https://github.com/WinMerge/winmerge/issues/2566))

#### アーカイブサポート

- 7-Zip をバージョン24.09 に更新した。

### 2024/11/29 2.16.44-jp-3

#### 全般

- 不具合修正: WinMergeをセカンドモニターで最大化表示するとタイトルバーの高さが大きくなりすぎる問題を修正した。([#2510](https://github.com/WinMerge/winmerge/issues/2510), [#2512](https://github.com/WinMerge/winmerge/issues/2512), [#2540](https://github.com/WinMerge/winmerge/issues/2540), [#2549](https://github.com/WinMerge/winmerge/issues/2549))
- 不具合修正: WinMergeの最大化表示時に右上端にマウスカーソルを移動したとき、閉じるボタンが押せない問題を修正した。([#2520](https://github.com/WinMerge/winmerge/issues/2520))
- 不具合修正: タスクバー自動非表示に設定している場合、WinMergeの最大化表示時にマウスカーソルを下端に移動しても、タスクバーが表示されない問題を修正した。([#2518](https://github.com/WinMerge/winmerge/issues/2518))
- 非アクティブ時にタイトルバーの色やアイコンを灰色にするようにした。([PR #2497](https://github.com/WinMerge/winmerge/pull/2497))([PR #2544](https://github.com/WinMerge/winmerge/pull/2544))([PR #2545](https://github.com/WinMerge/winmerge/pull/2545))([PR #2547](https://github.com/WinMerge/winmerge/pull/2547))(PRをいただきました。ありがとうございます。)
- Windowsの[タイトルバーとウィンドウ枠線にアクセントカラーを付ける]の設定を反映するようにした。([PR #2505](https://github.com/WinMerge/winmerge/pull/2505))(PRをいただきました。ありがとうございます。)
- メニューバーを非表示にできるようにした。([PR #2509](https://github.com/WinMerge/winmerge/pull/2509))(PRをいただきました。ありがとうございます。)

#### ファイル比較

- 不具合修正: 選択されたテキスト内の差異を右側または左側にコピーする際に想定外のテキストがコピーされることがある問題を修正した。([#2499](https://github.com/WinMerge/winmerge/issues/2499))
- 不具合修正: [表示]→[ペインをロック]メニューがチェックされている場合、デュアルモニター間で WinMerge をリサイズすると正しく描画されない問題を修正した。([#2514](https://github.com/WinMerge/winmerge/issues/2514))
- 不具合修正: "Cascadia Mono" フォントのスタイルをRegular以外にした場合、文字幅が異常になる問題を修正した。([#2525](https://github.com/WinMerge/winmerge/issues/2525))
- 不具合修正: ロケーションペイン内で移動ブロックをつなぐ線の高さが正しくない場合があったのを修正した。
- 不具合修正: App-V上でWinMergeを起動後、2つのファイルをドラッグ＆ドロップで開くとクラッシュする問題の対策([#2548](https://github.com/WinMerge/winmerge/issues/2548))
- 不具合修正: 左ペインまたは右ペインの内容をすべて削除して更新すると、"Debug Assertion Failed!" エラーが発生することがある問題を修正した。([#2556](https://github.com/WinMerge/winmerge/issues/2556))
- マウス右ボタン＋ホイールスクロール操作時に右ボタンを離したときの処理を改善した。([PR #2511](https://github.com/WinMerge/winmerge/pull/2511))(PRをいただきました。ありがとうございます。)
- コンテキストメニュー表示中に[選択した差異(左/右側)をクリップボードにコピー]を `1` ～ `3` キーで選択できるようにした。([PR #2532](https://github.com/WinMerge/winmerge/pull/2532))(PRをいただきました。ありがとうございます。)
- キャレットの幅を Windows の設定に従うようにした。([PR #2534](https://github.com/WinMerge/winmerge/pull/2534))(PRをいただきました。ありがとうございます。)
- 検索ダイアログや置換ダイアログの"検索する文字列" と "置換後の文字列" のテキスト入力エリアのフォントを現在選択中の固定幅フォントにするようにした。([#2539](https://github.com/WinMerge/winmerge/issues/2539))

#### フォルダー比較

- 不具合修正: 比較中にキー入力するとクラッシュすることがある問題を修正した。([#1814](https://github.com/WinMerge/winmerge/issues/1814), [PR #2557](https://github.com/WinMerge/winmerge/pull/2557))(PRをいただきました。ありがとうございます。)

#### オプションダイアログ

- オプションダイアログの[色/システム]カテゴリに "デフォルト" ボタンを追加した。 ([PR #2506](https://github.com/WinMerge/winmerge/pull/2506))(PRをいただきました。ありがとうございます。)
- オプションダイアログの[シェル統合]カテゴリの"すべての最近使用したものの履歴をクリアする" ボタンが、ジャンプリストに加えコンボボックス履歴もクリアするようした。([#2555](https://github.com/WinMerge/winmerge/issues/2555))

#### ファイルまたはフォルダを選択ダイアログ

- 不具合修正: "ファイルまたはフォルダを選択" ウィンドウで無効なファイルパスを指定するとクラッシュする場合があるのを修正した。

#### プラグイン

- Apache Tika プラグイン - Apache Tika を 3.0.0 にアップデート

#### インストーラー

- 不具合修正: WinMerge をアンインストールしても、Windows 11 用のシェルエクステンションが削除されない問題を修正した。
- サイレントインストール時、PowerShell を非表示で `-NoProfile` オプション付きで実行するようにした。([#2515](https://github.com/WinMerge/winmerge/issues/2515))

### 2024/10/29 2.16.44-jp-1

#### 全般

- タイトルバー上にタブバーを配置できるようにした。(Windows10以上のみ有効。これをデフォルトにしています。[表示]→[タブバー]→[タイトルバー上に配置\]メニューのチェックを外すと以前と同じ配置になります。) ([PR #2428](https://github.com/WinMerge/winmerge/pull/2428))
- マウス右ボタン+マウスホイールで次/前の差異への移動やマージができるようにした。 ([PR #2435](https://github.com/WinMerge/winmerge/pull/2435))(PRをいただきました。ありがとうございます。)
- システムカラーを上書きしてツールバーやステータスバー等の色を変えられるようにした。(カラースキームの変更とも連動しています) ([PR #2376](https://github.com/WinMerge/winmerge/pull/2376))
- タイトルバーにタブがある場合に左側WinMergeアイコンの右側をドラッグできるようにした。 ([PR #2489](https://github.com/WinMerge/winmerge/pull/2489))(PRをいただきました。ありがとうございます。)
- ツールバーのアイコンとして中サイズを選択できるようにした。

#### ファイル比較

- 不具合修正: TeXファイルのシンタックスハイライトの誤りを修正した。 ([#2415](https://github.com/WinMerge/winmerge/issues/2415))
- 不具合修正: テキスト置換の結果が正しくないことがある問題を修正した。 ([#2422](https://github.com/WinMerge/winmerge/issues/2422))
- 選択された差異をクリップボードにコピーする機能を追加した。 ([PR #2429](https://github.com/WinMerge/winmerge/pull/2429))(PRをいただきました。ありがとうございます。)
- Ada言語のシンタックスハイライトを追加した。 ([PR #2452](https://github.com/WinMerge/winmerge/issues/2452))(PRをいただきました。ありがとうございます。)
- C++20モジュール用のファイル関連付け(cppmとixx)を追加した。 ([PR #2464](https://github.com/WinMerge/winmerge/pull/2464))(PRをいただきました。ありがとうございます。)
- ロケーションペインで移動ブロックを接続する線にアンチエイリアスが適用されるようにした。

#### フォルダー比較

- 不具合修正: /enableexitcode コマンドラインオプション使用時、比較エラーが発生していないにもかかわらず、プロセスの終了ステータスが2となることがある問題を修正した。 ([#2450](https://github.com/WinMerge/winmerge/issues/2450))

#### Webページ比較

- 不具合修正: ロケーションペインで差異が正しく表示されないことがある問題を修正した。(winwebdiff[#6](https://github.com/WinMerge/winmerge/issues/6)) (winwebdiff[#7](https://github.com/WinMerge/winmerge/issues/7))

#### オプションダイアログ

- 「オプション(コードページ)」ダイアログに「デフォルト」ボタンを追加した。 ([PR #2448](https://github.com/WinMerge/winmerge/pull/2448))(PRをいただきました。ありがとうございます。)
- 「オプション(一般)」ダイアログに「デフォルト」ボタンを追加した。 ([PR #2453](https://github.com/WinMerge/winmerge/pull/2453))(PRをいただきました。ありがとうございます。)

#### アーカイブサポート

- 7-Zip バージョン 24.08に更新した。

#### プラグイン

- Java の properties ファイル比較用プラグイン CompareEscapedJavaPropertiesFiles.sct を追加した。 ([PR #2455](https://github.com/WinMerge/winmerge/pull/2455))(PRをいただきました。ありがとうございます。)
- 不具合修正: CompareMSExcelFiles.sctプラグイン: 数式の計算結果として 6,05ではなく、6.050000000000001 のように表示されることがある問題を修正した。 ([#2494](https://github.com/WinMerge/winmerge/issues/2494))

#### マニュアル

- 不具合修正: マニュアルのデフォルト値に関する2箇所の誤りを修正した。 ([#2456](https://github.com/WinMerge/winmerge/issues/2456))

### 2024/08/29 2.16.42-jp-3

#### 全般

- メニューバーをツールバーとして実装した。 [(PR #2400)](https://github.com/WinMerge/winmerge/pull/2400)
- 「WinMerge について」ウインドウでバージョン情報をテキスト選択できるようにした。

#### オプションダイアログ

- 不具合修正: (比較 > 画像) カテゴリーの「画像ファイルとして扱うパターン」を空欄にすると、すべてのファイルが画像として扱われてしまう問題を修正した。[(#2408)](https://github.com/WinMerge/winmerge/issues/2408)
- (プロジェクト) カテゴリーに「デフォルト」ボタンを追加した。 [(PR #2401)](https://github.com/WinMerge/winmerge/pull/2401)(PRをいただきました。ありがとうございます。)
- (システム) カテゴリーに「デフォルト」ボタンを追加した。 [(PR #2405)](https://github.com/WinMerge/winmerge/pull/2405)(PRをいただきました。ありがとうございます。)
- (バックアップ) カテゴリーに「デフォルト」ボタンを追加した。 [(PR #2406)](https://github.com/WinMerge/winmerge/pull/2406)(PRをいただきました。ありがとうございます。)

#### マニュアル

- オプション「片方に存在しないサブフォルダー内も含める」のデフォルト値の誤りを修正した。 [(PR #2396)](https://github.com/WinMerge/winmerge/pull/2396)(PRをいただきました。ありがとうございます。)

### 2024/07/29 2.16.42-jp-2

#### 全般

- Windows11上でメニューが角丸になるようにした。[(PR #2364)](https://github.com/WinMerge/winmerge/pull/2364)
- ステータスバーの分割線を描画しないようにした。[(PR #2377)](https://github.com/WinMerge/winmerge/pull/2377)

#### フォルダー比較

- 不具合修正: フォルダー比較のステータスがツールバーに正確に反映されていなかった問題を修正した。[(#2374)](https://github.com/WinMerge/winmerge/issues/2374)
- 不具合修正: 再読み込み(F5)後にタブアイコンがフォルダー比較のステータスを正しく反映していなかった問題を修正した。[(#2383)](https://github.com/WinMerge/winmerge/issues/2383)

#### ファイル比較

- ファイル全体と選択範囲の置換をより賢く選択するように置換機能を変更した。[(#2368)](https://github.com/WinMerge/winmerge/issues/2368)

#### 画像比較

- 不具合修正: 画像比較でオーバーレイアニメーション中にダイアログがフリーズする問題を修正した。[(#2370)](https://github.com/WinMerge/winmerge/issues/2370)
- ステータスバーの右端が白く表示される問題を修正した。
- 点滅間隔やオーバーレイアニメーション間隔を変更できるようにした。

#### プラグイン

- AIConvertTextプラグイン設定ウィンドウでgpt4-o-miniモデルを選択可能にした。

#### アーカイブサポート

- 7-Zip 24.07 に更新した。

### 2024/06/29 2.16.40-jp-3

#### 全般

- タブバーのタブを、Firefox のように角丸にした。
- Windows11上でメニューが角丸になるようにした。(PR #2364)

#### フォルダー比較

- 不具合修正: [選択項目を最新に更新]をクリックして再比較した際、比較進捗ウインドウに選択していないファイル名が表示される問題を修正した。 [(#2338)](https://github.com/WinMerge/winmerge/issues/2338)
- 不具合修正: ファイルやフォルダ等を選択している状態でフォルダを展開すると別のファイルやフォルダが選択されることがある問題を修正した。[(#2359)](https://github.com/WinMerge/winmerge/issues/2359)

#### オプションダイアログ

- 不具合修正: (色 > テキスト)カテゴリーの"テキストの色をカスタマイズする" を変更するとキャンセルしても(色 > シンタックス) カテゴリの設定がデフォルトに戻ってしまう問題を修正した。[(#2355)](https://github.com/WinMerge/winmerge/issues/2355)
- (エディタ > 比較/マージ) カテゴリーに「デフォルト」ボタンを追加した。 [(PR #2348)](https://github.com/WinMerge/winmerge/pull/2348)(PRをいただきました。ありがとうございます。)
- (アーカイブサポート)カテゴリーに「デフォルト」ボタンを追加した。[(PR #2362)](https://github.com/WinMerge/winmerge/pull/2362)(PRをいただきました。ありがとうございます。)

### 2024/05/31 2.16.40-jp-2

#### 全般

- ファイルまたはフォルダーの選択ウインドウを表示した後、WinMergeを終了させてもプロセスが残りっぱなしになることがある問題を修正した。

#### ファイル比較

- TypeScript ファイルにJavaScriptシンタックスハイライトを適用するようにした。 [(PR#2312)](https://github.com/WinMerge/winmerge/pull/2312)(PRをいただきました。ありがとうございます。)
- F# シンタックスハイライトの改善。 [(PR#2303)](https://github.com/WinMerge/winmerge/pull/2303)[(PR#2309)](https://github.com/WinMerge/winmerge/pull/2309)(PRをいただきました。ありがとうございます。)

#### テーブル比較

- 行末近くの文字にカレットが移動できないことがある問題を修正した。

#### フォルダー比較

- ステータスバーをクリックするとファイル比較方法やファイルフィルターを変更できるようにした。

#### HTMLレポート

- 不具合修正: ファイル名に#を含む画像の比較レポートで画像が表示されない問題を修正した。[osdn#46082](https://osdn.net/projects/winmerge-jp/ticket/78171)

#### プラグイン

- AIConvertText プラグインを追加した。 [(PR#2258)](https://github.com/WinMerge/winmerge/pull/2258) (OpenAI API を使用して、指示した通りテキストを変換します。利用には OpenAI API Key の取得が必要になります)
- md4c 0.5.2 に更新した。
- jq 1.7.1 に更新した。

#### アーカイブサポート

- 7-Zip 24.05 に更新した。

#### その他

- GitHub Actions CI の更新。 [(PR#2304)](https://github.com/WinMerge/winmerge/pull/2304)(PRをいただきました。ありがとうございます。)
- Typo 修正。 [(PR#2305)](https://github.com/WinMerge/winmerge/pull/2305)(PRをいただきました。ありがとうございます。)
- Boost 1.85 に更新。
- POCO C++ Libraries 1.13.3 に更新。
- Google C++ Testing Framework 1.14.0 に更新。

### 2024/04/29 2.16.40-jp-1

#### 全般

- 不具合修正: Wine上で発生する不具合をいくつか修正した。

#### ファイル比較

- 不具合修正: テキストを選択状態にした後に置換すると正しく置換されないことがある問題を修正した。 [(#2279)](https://github.com/WinMerge/winmerge/issues/2279)
- F# シンタックスハイライトを追加した。 [(PR#2298)](https://github.com/WinMerge/winmerge/pull/2298)(PRをいただきました。ありがとうございます。)

#### オプションダイアログ

- "オプション (エディター > 一般)" ダイアログに "デフォルト" ボタンを追加した。 [(PR #2283)](https://github.com/WinMerge/winmerge/pull/2283)(PRをいただきました。ありがとうございます。)
- "オプション > 比較 > テーブル" 内の "デフォルト" ボタンの位置を調整した。 [(PR #2295)](https://github.com/WinMerge/winmerge/pull/2295)(PRをいただきました。ありがとうございます。)

#### プラグイン

- 不具合修正: CompareMSExcelFiles.sct: 'ワークブックの情報を複数ファイルに展開する' オプションが有効になっている場合、10枚以上のシートを含む .xlsx ファイルのすべてのシートが比較されない問題を修正した。(このバグはバージョン2.16.39 ベータで発生しました。)
- 不具合修正: insert datetime.sct: 地域によっては正常に動作しなかった問題を修正した。(このバグはバージョン2.16.39 ベータで発生しました。)
- 不具合修正: ファイルとフォルダーの選択ウィンドウが表示されているときにプラグインを再読み込みすると "Catastrophic failure" メッセージボックスが表示される可能性がある問題を修正した。
- GUI にプラグインパイプラインのエイリアスまたは単純なプラグインを登録できるようにした。 [(PR #2257)](https://github.com/WinMerge/winmerge/pull/2257)

#### インストーラー

- 不具合修正: 不具合修正: インストールの最後(最後のダイアログボックス)でのフランス語のエンコーディングの問題を修正した。 [(#2272)](https://github.com/WinMerge/winmerge/issues/2272)

### 2024/03/29 2.16.38-jp-3

#### 全般

- 不具合修正: ヘッダーバーに1文字だけを入力するとクラッシュすることがある問題を修正した。

#### ファイル比較

- 不具合修正: クラッシュする可能性がある箇所を修正した。
- 不具合修正: 元のファイル名がドットで始まる場合、.bak ファイルの作成が失敗する問題を修正した。[(#2217)](https://github.com/WinMerge/winmerge/issues/2217)
- Java シンタックスハイライトのキーワードを更新した。 [(PR#2215)](https://github.com/WinMerge/winmerge/pull/2215)(PRをいただきました。ありがとうございます。)
- テキストを選択した状態で「右にコピー」等で別ペインにコピーする際の粒度を「差異ブロック」、「行内差異」、「行」、「文字」から選択できるようにした。
  (オプションウインドウの[エディター/比較/マージ]カテゴリの[選択された差異のコピー粒度]で選択できます)[(PR#2224)](https://github.com/WinMerge/winmerge/pull/2224)
- 「右側へコピー」または「左側へコピー」でコピーするテキストをプラグインで加工できるようにした。
   ([プラグイン]→[コピー時適用エディタースクリプト]メニューでプラグインを選択できます) [(PR#2238)](https://github.com/WinMerge/winmerge/pull/2238)
- PHP シンタックスハイライトのキーワードを更新した。 [(PR#2265)](https://github.com/WinMerge/winmerge/pull/2265)(PRをいただきました。ありがとうございます。)

#### Webページ比較

- 不具合修正: ロケーションペインで[イベント同期]等の設定を変更しても、次回起動時に反映されない問題を修正した。 [(#2248)](https://github.com/WinMerge/winmerge/issues/2248)

#### ファイルまたはフォルダーの選択ウインドウ

- アーカイブファイルと通常ファイルを指定した場合に比較ボタンが押せない問題を修正した。

#### HTMLレポート

- 不具合修正: HTML レポートの左ペインと右ペインの幅が等しくないことがある問題を修正した。
- 不具合修正: ヘッダー バーに設定されたキャプションが HTML レポートに適用されない問題を修正した。

#### プラグイン

- 不具合修正: 展開プラグインでエラーが発生したとき、クラッシュする問題を修正した。
- VBScriptが非推奨となったため、プラグインをJScriptで書きなおした。 [(PR#2217)](https://github.com/WinMerge/winmerge/pull/2217)
- 置換フィルターのパターンを使用して置換する機能を置換プラグインに追加した。 (Replace プラグインに -s オプションを指定します) [(PR#2252)](https://github.com/WinMerge/winmerge/pull/2252)
- PrediffLineFilter プラグイン正規表現の正常性チェックを追加した。

#### インストーラー

- 不具合修正: 前回のインストールで /noicons オプションが指定されていた場合、次回のインストール時に以前のスタート メニューを削除するように求めるメッセージ ボックスが表示されてしまう問題を修正した。[(#2206)](https://github.com/WinMerge/winmerge/issues/2206)

#### アーカイブサポート

- ファイル名を暗号化して圧縮した 7z ファイルを比較できない問題を修正した。[(#2225)](https://github.com/WinMerge/winmerge/issues/2225)


### 2024/01/29 2.16.38-jp-1

#### ファイル比較

- 不具合修正: コードページダイアログで右側のBOMを変更しても反映されない問題を修正した。
- C++ シンタックスハイライトのキーワードを更新した。 [(PR#2166)](https://github.com/WinMerge/winmerge/pull/2166)(PRをいただきました。ありがとうございます。)

#### Webページ比較

- 比較中はステータスバーに「比較しています...」を表示するようにした。
- ロケーションペインを追加した。 [(PR#2160)](https://github.com/WinMerge/winmerge/pull/2160)

#### フォルダー比較

- [列の表示]ダイアログのボタンの活性/非活性制御の改善。 [(PR#2154)](https://github.com/WinMerge/winmerge/pull/2154)(PRをいただきました。ありがとうございます。)

#### プラグイン

- 不具合修正: 以下のように二重引用符を文字列が `/unpacker` コマンドライン引数に指定された場合に正しく解釈されない問題を修正した。
  
    `/unpacker "Replace ""a"" ""b"""`

