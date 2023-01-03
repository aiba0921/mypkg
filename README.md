# mypkg
  * このリポジトリは千葉工業大学未来ロボティクス学科2年後期のロボットシステム学の講義で扱っているros2のパッケージです。
  * このリポジトリには
    * talker.py
    * listener.py

    があります

![test](https://github.com/aiba0921/mypkg/actions/workflows/test.yml/badge.svg)
## 動作確認済み環境
  * Ubuntu 20.04.5 LTS
  * ROS2 Humble

## リポジトリの概要
  * talker.py
    * countupというトピックを用いて16ビットの符号付き整数を送信する
    
  * listener.py
    * countupからメッセージを受信し、出力する側
  
  * talk_listen.launch.py
    * このパッケージにあるノードを一度に立ち上げる
    
## 実行方法
  * ````$ cd mypkg````でディレクトリに移動
  * 入出力
    ````
    $ ros2 launch mypkg talk_listen.launch.py
    [INFO] [launch]: All log files can be found below /home/aibay/.ros/log/2023-01-03-12-59-26-144435-DESKTOP-4DPTDA2-1334
    [INFO] [launch]: Default logging verbosity is set to INFO
    [INFO] [talker-1]: process started with pid [1335]
    [INFO] [listener-2]: process started with pid [1337]
    [listener-2] [INFO] [1672718366.890392600] [listener]: Listen: 0
    [listener-2] [INFO] [1672718367.380941300] [listener]: Listen: 1
    [listener-2] [INFO] [1672718367.880556700] [listener]: Listen: 2
    [listener-2] [INFO] [1672718368.381355900] [listener]: Listen: 3
    [listener-2] [INFO] [1672718368.881343600] [listener]: Listen: 4
    [listener-2] [INFO] [1672718369.381606900] [listener]: Listen: 5
    [listener-2] [INFO] [1672718369.881293100] [listener]: Listen: 6
    [listener-2] [INFO] [1672718370.381408900] [listener]: Listen: 7
    [listener-2] [INFO] [1672718370.879201700] [listener]: Listen: 8
    [listener-2] [INFO] [1672718371.378691200] [listener]: Listen: 9
    [listener-2] [INFO] [1672718371.878899200] [listener]: Listen: 10

## ライセンス
  * このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
  * このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．
      * [ryuichiueda/my_slides robosys_2022](https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022)
  * © 2022 Yuto Aiba
