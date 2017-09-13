# MaruBatsu

## 概要
CPUとマルバツゲームの対戦ができるJavaアプリケーション。強化学習（Q学習）による戦略も実装。

## 更新履歴
|ver.|更新日|内容|
|:-|:-|:-|
|1.0|2017/09/13|初版。|

## ファイル構成
#### ソースファイル
- MaruBatsuMain.java:マルバツゲームのメインクラス。
- MaruBatsuBasic.java:マルバツゲームの基本データクラス。
- MaruBatsuGUI.java:マルバツゲームの画面処理を行うクラス。
- MaruBatsuQlearning.java:Q学習の戦略を行うクラス。
- MaruBatsuTest.java:CPUの各戦略の比較を行うクラス。
- ConvertBasicNum.java:Q学習で用いる基数変換クラス。

#### 実行ファイル
- MaruBatsuMain.java:マルバツゲームを開始するときに実行。
- MaruBatsuTest.java:CPUの各戦略の比較を行うときに実行。

## CPUの各戦略の紹介
- ランダム:ランダムに行動する。※起動時のデフォルトはランダム戦略。
- 簡易戦略:縦横斜めで一方の記号が2つ以上並んでいる、かつ、最後の1つが空いていればそこにマークする。それ以外はランダムに行動する。
- Q学習:任意回数分Q学習後の戦略で行動する。  
