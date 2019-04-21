# Re:VIEWテンプレート

## 概要説明
ワンストップ　タイムマネジメント

## この本の目的
パパエンジニア、ママエンジニアの執筆時間捻出や時短家事に関するノウハウ集。

どうやって時間捻出してます？
家族の時間、自分の時間、本業の時間、そのスキマを縫って本を書く時間を捻出する。
頭が下がります。

というわけで、そんなあなたのテクニックを共有しませんか？



## 執筆・配布スケジュール
募集開始・環境構築　4月21日  
章目次確定：5月15日  
本文初稿：5月末  
レビュー＆追記： 6月末日  
入稿:7月20日
発行　夏コミ(日程、募集開始はまだですが)
を大枠なスケジュールとします。(多少前後します。極力前倒しはないようにします。)

## 著者紹介兼あとがき
Contributers.re内に、テンプレートに従って記入ください。

## 執筆にあたってのお願い
CIでコンパイルが通ることを確認してください。エラーのまま放置はなるべくやめてください。

Confrictが発生した場合は、解決お願いします。

push -f等はやめましょう。（歴史を書き換えてはいけません。

相談事：
Issue立ててください。

雑談、ざっくばらんな相談については、Slackがあります。
参加方法は、親方まで。https://twitter.com/oyakata2438/
## Re:VIEWの書き方

[Re:VIEWチートシート](https://gist.github.com/erukiti/c4e3189dda179a0f0b73299fb5787838) を作ってくれたみたので、参考にしてみてください。

## CI
https://app.wercker.com/oyakata2438/Onestop-timeManagement/runs
でPDFが書きだされます。
一番上のBuildをクリックすると展開されるので、
Output Artifactをクリックして、Download artifactをクリックすると、
tarで固めたpdfがダウンロードできます。

## インストール

細かい準備(TeX入れたり)は[『技術書をかこう！』](https://github.com/TechBooster/C89-FirstStepReVIEW-v2)に準じます。

### WindowsでReviewを使う方法

https://qiita.com/implicit_none/items/398c6e0bbedc8b160621
暗黙の型宣言さんが詳しく書いてくれてます。あるいは、技術同人誌を書こう‐アウトプットのススメ‐をご覧ください。

### Dockerを使う方法

Dockerを使うのが一番手軽です。

```sh
$ docker run --rm -v `pwd`:/work vvakame/review /bin/sh -c "cd /work/articles ; review-pdfmaker config.yml"
```

### Docker使わずビルド

```sh
cd articles ; review pdfmaker config.yml
```

> Visual Studio Code で `Onestop-meeting` フォルダーを開くと、ビルドタスク `Build PDF with Re:VIEW` を使ってこのコマンドを実行できます。

### 権利

ベースには、[TechBooster/ReVIEW\-Template: TechBoosterで利用しているRe:VIEWのテンプレート（B5/A5/電子書籍）](https://github.com/TechBooster/ReVIEW-Template) を使っています。

  * 設定ファイル、テンプレートなど制作環境（techbooster-doujin.styなど）はMITライセンスです
    * 再配布などMITライセンスで定める範囲で権利者表記をおねがいします
