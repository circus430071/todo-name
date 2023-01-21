## a
* 時間を管理できるソフトを作りたい(タイマーに毛が生えた程度のもの)
* ポモドーロ法のような時間管理方法(一応他の方法もあるか調べる)　
* 今スマホ使ってるやつが画面遷移に対応してなくて使いにくい
* ガチな物は書かない(複雑な機能、UI等)　メンテ、開発等、時間をあまりこれに割けない。　かといってその辺で依頼すると鬼高い上に品質が微妙になる
* 機能の案は他にもあるが、全てをここには書かない（これがメイン　どうしても実現したい）

以前書きかけたが機能を欲張りすぎてごちゃごちゃになって面倒になった
二回目なのである程度勘が働く

## 要件
* Android, Linux Desktop環境で動く(できればWindowsも)

## 道具検討
||利点|欠点|
|---|---|---|
|C++ & Qt|動作が速い　QMLがクロスプラットフォーム|開発効率△~×(多機能なUIとか作ろうとすると死ぬほど時間がかかる)　　Qt&QMLである程度複雑なことをしようとするとごちゃってきてきつくなる|
|C# & [Avalonia](https://www.avaloniaui.net/)|UIがモダン　C#自体が比較的ハイレベル　UIのパーツが揃ってそうなのでちょっと手の込んだ機能も比較的簡単に実現できそう|QtよりもっさりするUIができそう|


~~2. Flatter(?) + android studio kotolinとかそのへん つかったことねえ
https://tauri.app/blog/2022/12/09/tauri-mobile-alpha/#updating-dependencies　(新しいのでトラブりそう)
最悪Dekstopだけで動けばいいかもしれない　その場合xamarin(?)もありか？~~

### メモ
https://docs.avaloniaui.net/tutorials/developing-for-mobile/create-a-cross-platform-solution


## ポモドーロ法について
https://ja.wikipedia.org/wiki/%E3%83%9D%E3%83%A2%E3%83%89%E3%83%BC%E3%83%AD%E3%83%BB%E3%83%86%E3%82%AF%E3%83%8B%E3%83%83%E3%82%AF
```
具体的な手順は以下の通りである。

    達成しようとするタスクを選ぶ
    キッチンタイマーで25分を設定する
    タイマーが鳴るまでタスクに集中する
    少し休憩する（5分程度）
    ステップ2 - 4を4回繰り返したら、少し長めに休憩する（15分 - 30分）

ポモドーロの途中で急用が入りタスクが中断された場合は、そのポモドーロは終了とみなし、はじめから新しいポモドーロを開始する。

メールをチェックしたくなったり、誰かに連絡する用事を急に思い出したり、他人を気にしたりしてタスクを中断することは「内的中断」であり、さほど重要でないことをやっており、そもそもの目標設定が適切でないことに原因があるとしている。

ポモドーロ・テクニックは開発者、デザイナーなどクリエイティブな職業に就く人から支持されている。 
```
