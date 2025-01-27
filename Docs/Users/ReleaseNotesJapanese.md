# WinMerge 2.16.46 リリースノート

- [このリリースについて](#about-this-release)
- [2.16.46 の新機能](#what-is-new-in-21646)
- [2.16.45.1 beta の新機能](#what-is-new-in-216451-beta)
- [2.16.45.0 beta の新機能](#what-is-new-in-216450-beta)
- [既知の問題](#known-issues)

2025年1月

## このリリースについて

WinMerge の 2.16.46 安定版リリースです。
このリリースは、以前の WinMerge 安定版リリースに代わる推奨リリースです。

不具合は <a href="http://github.com/WinMerge/winmerge/issues">bug-tracker</a> で報告してください。
日本語での報告は、<a href="https://sourceforge.net/p/winmerge-v2-jp/tickets/">こちら</a>でお願いします。

## <a name="what-is-new-in-21644"></a>2.16.46 の新機能

### 全般

- 不具合修正: Al+F4キーで WinMerge が終了せずにツールメニューが表示される問題を修正した。（[#2592](https://github.com/WinMerge/winmerge/issues/2592)）。  
- 不具合修正: Windowsのアニメーション効果が有効な状態でWinMergeを最大化して起動すると、一瞬タイトルバーの描画位置がずれる問題を修正した。

### フォルダー比較

- 不具合修正: 左右のファイル名の大文字小文字も異なる場合、片方のファイルを削除後残ったファイルを反対側にコピーするとファイル名の大文字小文字が一致しない問題を修正した。（[#2599](https://github.com/WinMerge/winmerge/issues/2599)）。  
- フォルダー比較ウインドウで左側から右側または逆方向にコピーする際、選択された項目に同一ファイルやスキップされたファイルが含まれていた場合に差異のあるファイルのみをコピーするか確認するダイアログを表示するようにした。（[PR #2622](https://github.com/WinMerge/winmerge/pull/2622)）。

### プラグイン

- 不具合修正: バージョン2.16.43以降、プラグイン -> 比較前処理プラグイン メニューが正しく表示されない問題を修正した。  
- 不具合修正: PowerPoint ファイルを CompareMSPowerPointFiles.sct プラグインで比較するとエラー 0x80048010 が発生することがある問題を修正した。
- ファイル番号を指定してプラグインを適用できる機能を追加した。（[PR #2598](https://github.com/WinMerge/winmerge/pull/2598)）。  
- プラグインウィンドウをリサイズ可能にした。プラグインの種類ごとに表示するようにした。（[PR #2621](https://github.com/WinMerge/winmerge/pull/2621)）。

### マニュアル

- 不具合修正: WinMergeマニュアル内の誤字を修正した（[#2597](https://github.com/WinMerge/winmerge/issues/2597)）

### 翻訳

- 翻訳の更新:
  - Brazilian (PR #2601,#2623)
  - Chinese Simplified (PR #2603,#2624) 
  - French (PR #2595,#2612)
  - Hungarian (PR #2602)
  - Italian (PR #2610,#2627)
  - Japanese
  - Korean (PR #2611,#2630)
  - Lithuanian (PR #2604,#2628)
  - Portuguese (PR #2614)
  - Russian (PR #2593,#2609,#2629)

## <a name="what-is-new-in-216451"></a>2.16.45.1 Beta の新機能

### 全般

- 不具合修正: メニューが非表示の場合、Shift+Altキーで言語を切り替えると、メニューにフォーカスが当たってしまう問題を修正した。
  ([PR #2572](https://github.com/WinMerge/winmerge/pull/2572))(PRをいただきました。ありがとうございます。)
- オプションダイアログの[比較/一般]カテゴリに[ファイル末尾の改行文字の有無を無視する」オプションを追加した。
  ([PR #2573](https://github.com/WinMerge/winmerge/pull/2573), [#203](https://github.com/WinMerge/winmerge/issues/203), [#989](https://github.com/WinMerge/winmerge/issues/989), [#2317](https://github.com/WinMerge/winmerge/issues/2317))

### ファイル比較

- 不具合修正: ロケーションペイン内の移動ブロックをつなぐ線の高さが正しくない場合がある問題を修正した。
  ([#2543](https://github.com/WinMerge/winmerge/issues/2543))

### フォルダー比較

- 不具合修正: フォルダー比較が完了する前にフォルダーアイコンに緑のチェックマークが付く問題を修正した。  
  ([#2562](https://github.com/WinMerge/winmerge/issues/2562))

### プラグイン

- 不具合修正: CompareMSWordFiles プラグイン: RTFファイルを比較すると変換確認ウインドウが表示される問題を修正した。 
  ([#2566](https://github.com/WinMerge/winmerge/issues/2566))

### アーカイブサポート

- 7-Zip をバージョン24.09 に更新した。

### 翻訳

- 翻訳の更新:
  - Brazilian (PR #2585)
  - Chinese Simplified (PR #2588) 
  - Hungarian (PR #2586)
  - Italian (PR #2587)
  - Lithuanian (PR #2591)
  - Japanese
  - Korean (PR #2558,#2559)

## その他

- POCO C++ Libraries を 1.14.0 に更新した。

## <a name="what-is-new-in-216450"></a>2.16.45.0 Beta の新機能

### 全般

- 不具合修正: WinMergeをセカンドモニターで最大化表示するとタイトルバーの高さが大きくなりすぎる問題を修正した。([#2510](https://github.com/WinMerge/winmerge/issues/2510), [#2512](https://github.com/WinMerge/winmerge/issues/2512), [#2540](https://github.com/WinMerge/winmerge/issues/2540), [#2549](https://github.com/WinMerge/winmerge/issues/2549))
- 不具合修正: WinMergeの最大化表示時に右上端にマウスカーソルを移動したとき、閉じるボタンが押せない問題を修正した。([#2520](https://github.com/WinMerge/winmerge/issues/2520))
- 不具合修正: タスクバー自動非表示に設定している場合、WinMergeの最大化表示時にマウスカーソルを下端に移動しても、タスクバーが表示されない問題を修正した。([#2518](https://github.com/WinMerge/winmerge/issues/2518))
- 非アクティブ時にタイトルバーの色やアイコンを灰色にするようにした。([PR #2497](https://github.com/WinMerge/winmerge/pull/2497))([PR #2544](https://github.com/WinMerge/winmerge/pull/2544))([PR #2545](https://github.com/WinMerge/winmerge/pull/2545))([PR #2547](https://github.com/WinMerge/winmerge/pull/2547))(PRをいただきました。ありがとうございます。)
- Windowsの[タイトルバーとウィンドウ枠線にアクセントカラーを付ける]の設定を反映するようにした。([PR #2505](https://github.com/WinMerge/winmerge/pull/2505))(PRをいただきました。ありがとうございます。)
- メニューバーを非表示にできるようにした。([PR #2509](https://github.com/WinMerge/winmerge/pull/2509))(PRをいただきました。ありがとうございます。)

### ファイル比較

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

### フォルダー比較

- 不具合修正: 比較中にキー入力するとクラッシュすることがある問題を修正した。([#1814](https://github.com/WinMerge/winmerge/issues/1814), [PR #2557](https://github.com/WinMerge/winmerge/pull/2557))(PRをいただきました。ありがとうございます。)

### オプションダイアログ

- オプションダイアログの[色/システム]カテゴリに "デフォルト" ボタンを追加した。 ([PR #2506](https://github.com/WinMerge/winmerge/pull/2506))(PRをいただきました。ありがとうございます。)
- オプションダイアログの[シェル統合]カテゴリの"すべての最近使用したものの履歴をクリアする" ボタンが、ジャンプリストに加えコンボボックス履歴もクリアするようした。([#2555](https://github.com/WinMerge/winmerge/issues/2555))

### ファイルまたはフォルダを選択ダイアログ

- 不具合修正: "ファイルまたはフォルダを選択" ウィンドウで無効なファイルパスを指定するとクラッシュする場合があるのを修正した。

### プラグイン

- Apache Tika プラグイン - Apache Tika を 3.0.0 にアップデート

### インストーラー

- 不具合修正: WinMerge をアンインストールしても、Windows 11 用のシェルエクステンションが削除されない問題を修正した。
- サイレントインストール時、PowerShell を非表示で `-NoProfile` オプション付きで実行するようにした。([#2515](https://github.com/WinMerge/winmerge/issues/2515))

### 翻訳

- 翻訳の更新:
  - Brazilian (PR #2526)
  - Chinese Simplified (PR #2501,#2524) 
  - French (PR #2536)
  - Hungarian (PR #2495,#2523)
  - Italian (PR #2529)
  - Japanese
  - Korean (PR #2496,#2533)
  - Lithuanian (PR #2503,#2537)
  - Portuguese (PR #2507)
  - Russian (PR #2500,#2502,#2521,#2522,#2528,#2531,#2538,#2542)

### その他

- Make InsertLineNumberInPOFiles.bat and RenewPOFiles.bat work again

## <a name="known-issues"></a>既知の問題

 - フォルダ比較で画像比較を有効にした場合、比較結果が安定しない。 [(#1391)](https://github.com/WinMerge/winmerge/issues/1391)
 - 巨大ファイルの比較でクラッシュすることがある。[(#325)](https://github.com/WinMerge/winmerge/issues/325)
 - 大幅に異なるフォルダの比較が非常に時間がかかる。 [(#322)](https://github.com/WinMerge/winmerge/issues/322)
 - 新規作成で表示範囲を超えるテキストを貼り付けたとき、垂直スクロールバーでスクロールできない。 [(#296)](https://github.com/WinMerge/winmerge/issues/296)
