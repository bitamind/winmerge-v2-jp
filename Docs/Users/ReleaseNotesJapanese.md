# WinMerge 2.16.44 リリースノート

- [このリリースについて](#about-this-release)
- [2.16.44 の新機能](#what-is-new-in-21644)
- [2.16.43 beta の新機能](#what-is-new-in-21643-beta)
- [既知の問題](#known-issues)

2024年10月

## このリリースについて

WinMerge の 2.16.44 安定版リリースです。
このリリースは、以前の WinMerge 安定版リリースに代わる推奨リリースです。

不具合は <a href="http://github.com/WinMerge/winmerge/issues">bug-tracker</a> で報告してください。
日本語での報告は、<a href="https://sourceforge.net/p/winmerge-v2-jp/tickets/">こちら</a>でお願いします。

## <a name="what-is-new-in-21644"></a>2.16.44 の新機能

### 全般

- ツールバーのアイコンとして中サイズを選択できるようにした。

### Webページ比較

- 不具合修正: ロケーションペインで差異が正しく表示されないことがある問題を修正した。(winwebdiff[#7](https://github.com/WinMerge/winmerge/issues/7))

### プラグイン

- 不具合修正: CompareMSExcelFiles.sctプラグイン: 数式の計算結果として 6,05ではなく、6.050000000000001 のように表示されることがある問題を修正した。 ([#2494](https://github.com/WinMerge/winmerge/issues/2494))

### 翻訳

- 翻訳の更新:
  - Brazilian (PR #2493)
  - Corsican (PR #2490)

## <a name="what-is-new-in-21643"></a>2.16.43 の新機能

### 全般

- 不具合修正: (比較 > 画像) カテゴリーの「画像ファイルとして扱うパターン」を空欄にすると、すべてのファイルが画像として扱われてしまう問題を修正した。[(#2408)](https://github.com/WinMerge/winmerge/issues/2408)
- メニューバーをツールバーとして実装した。 [(PR #2400)](https://github.com/WinMerge/winmerge/pull/2400)
- タイトルバーにタブがある場合に左側WinMergeアイコンの右側をドラッグできるようにした。 ([PR #2489](https://github.com/WinMerge/winmerge/pull/2489))(PRをいただきました。ありがとうございます。)
- マウス右ボタン+マウスホイールで次/前の差異への移動やマージができるようにした。 ([PR #2435](https://github.com/WinMerge/winmerge/pull/2435))(PRをいただきました。ありがとうございます。)
- システムカラーを上書きしてツールバーやステータスバー等の色を変えられるようにした。（カラースキームの変更とも連動しています） ([PR #2376](https://github.com/WinMerge/winmerge/pull/2376))
- タイトルバーにタブがある場合に左側WinMergeアイコンの右側をドラッグできるようにした。 ([PR #2489](https://github.com/WinMerge/winmerge/pull/2489))(PRをいただきました。ありがとうございます。)

### ファイル比較

- 不具合修正: TeXファイルのシンタックスハイライトの誤りを修正した。 ([#2415](https://github.com/WinMerge/winmerge/issues/2415))
- 不具合修正: テキスト置換の結果が正しくないことがある問題を修正した。 ([#2422](https://github.com/WinMerge/winmerge/issues/2422))
- 選択された差異をクリップボードにコピーする機能を追加した。 ([PR #2429](https://github.com/WinMerge/winmerge/pull/2429))(PRをいただきました。ありがとうございます。)
- Ada言語のシンタックスハイライトを追加した。 ([PR #2452](https://github.com/WinMerge/winmerge/issues/2452))(PRをいただきました。ありがとうございます。)
- C++20モジュール用のファイル関連付け（cppmとixx）を追加した。 ([PR #2464](https://github.com/WinMerge/winmerge/pull/2464))(PRをいただきました。ありがとうございます。)
- ロケーションペインで移動ブロックを接続する線にアンチエイリアスが適用されるようにした。

### フォルダー比較

- 不具合修正: /enableexitcode コマンドラインオプション使用時、比較エラーが発生していないにもかかわらず、プロセスの終了ステータスが2となることがある問題を修正した。 ([#2450](https://github.com/WinMerge/winmerge/issues/2450))

### Webページ比較

- 不具合修正: ロケーションペインで差異が正しく表示されないことがある問題を修正した。(winwebdiff[#6](https://github.com/WinMerge/winmerge/issues/6))

### オプションダイアログ

- 「オプション（コードページ）」ダイアログに「デフォルト」ボタンを追加した。 ([PR #2448](https://github.com/WinMerge/winmerge/pull/2448))(PRをいただきました。ありがとうございます。)
- 「オプション（一般）」ダイアログに「デフォルト」ボタンを追加した。 ([PR #2453](https://github.com/WinMerge/winmerge/pull/2453))(PRをいただきました。ありがとうございます。)

### アーカイブサポート

- 7-Zip 24.08 に更新した。

### プラグイン

- Java の properties ファイル比較用プラグイン CompareEscapedJavaPropertiesFiles.sct を追加した。 ([PR #2455](https://github.com/WinMerge/winmerge/pull/2455))(PRをいただきました。ありがとうございます。)

### Manual

- 不具合修正: マニュアルのデフォルト値に関する2箇所の誤りを修正した。 ([#2456](https://github.com/WinMerge/winmerge/issues/2456))
- オプション「片方に存在しないサブフォルダー内も含める」のデフォルト値の誤りを修正した。 [(PR #2396)](https://github.com/WinMerge/winmerge/pull/2396)(PRをいただきました。ありがとうございます。)

### 翻訳

- 翻訳の更新:
  - Brazilian (PR #2397,#2431,#2439,#2454,#2460,#2468,#2477,#2486)
  - Chinese Simplified (PR #2394,#2461,#2469,#2485)
  - Dutch (PR #2474)
  - French (PR #2399,#2444)
  - Hungarian (PR #2433,#2440,#2458,#2472,#2482)
  - Italian (PR #2393,#2438,#2446,#2447,#2457,#2467,#2470,#2487)
  - Japanese
  - Korean (PR #2426,#2459,#2473)
  - Lithuanian (PR #2436,#2443,#2462,#2471,#2483)
  - Portuguese (PR #2410,#2441,#2480)
  - Russian (PR #2462)

### Internals

- Make InsertLineNumberInPOFiles.bat and RenewPOFiles.bat work again

## <a name="known-issues"></a>既知の問題

 - フォルダ比較で画像比較を有効にした場合、比較結果が安定しない。 [(#1391)](https://github.com/WinMerge/winmerge/issues/1391)
 - 巨大ファイルの比較でクラッシュすることがある。[(#325)](https://github.com/WinMerge/winmerge/issues/325)
 - 大幅に異なるフォルダの比較が非常に時間がかかる。 [(#322)](https://github.com/WinMerge/winmerge/issues/322)
 - 新規作成で表示範囲を超えるテキストを貼り付けたとき、垂直スクロールバーでスクロールできない。 [(#296)](https://github.com/WinMerge/winmerge/issues/296)
