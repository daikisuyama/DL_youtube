# Deep Learningとは？

## 時間

2/2 10時ごろ

## DeepLearningの歴史

脳の学習機能をコンピューラーでシミュレーションするニューラルネットワークを用いた技術

脳では神経細胞がシナプス結合で結合し、結合間に電気信号が送信されることで脳の機能が実現されている
↓
人工ニューロン：$$y=f(\Sigma w_i x_i + b)$$(出力$y$,入力$x_i$)
神経細胞とシナプス結合を数理モデルにより再現する
↓
ニューラルネットワーク(多層パーセプトロン)
人工ニューロンを組み合わせることにより作成される
入力層→1~2層の中間層→出力層
↓
DeepLearning
中間層の数を多くした深いニューラルネットワーク
ニューロンの数も増える
従来は計算時間がかかるのと、学習しきるのには大量のデータが必要という問題
GPUにより並列計算の高速化
インターネットの普及により大量のデータを集められるように

## ニューラルネットワークの学習

e.g. MNISTデータセットによる手書き数字認識
→ 28*28の60000枚のモノクロの画像データを元に数字の識別を行う問題

入力ニューロンと出力ニューロンをそれぞれ用意し、適当な中間層を用意して学習を行わせる。
まず、ニューロン間の結合の重みを乱数で適当に初期化し、その後に出力が正解に近づくようにニューロン間の結合の重みを少しずつ更新する。
学習が進むにつれて正解の出力を出すように最適化される。