# mypkg
  * このリポジトリは千葉工業大学未来ロボティクス学科2年後期のロボットシステム学の講義で扱っているros2のパッケージです。
  * このリポジトリには
    * talker.py
    * listener.py

    があります

![test](https://github.com/aiba0921/mypkg/actions/workflows/test.yml/badge.svg)
## 動作確認済み環境
  * Ubuntu 20.04.5 LTS

## リポジトリの概要
  * talker.py
    * メッセージを送る側
    
  * listener.py
    * メッセージを受け受け取り、出力する側
    
## 実行方法
  * ````$ cd mypkg````でディレクトリに移動
  * 入出力
    ````
    $ ros2 launch mypkg talk_listen.launch.py
    [listener]:Listener: {実行時間}

## ライセンス
  * このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
  * このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
      * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)
  * © 2022 Yuto Aiba
