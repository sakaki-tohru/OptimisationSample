# GeneticAlgorithmSample

進化計算のサンプルプログラムです。
選択(淘汰)、交叉、突然変異、評価を繰り返すことで、目的の文字列(=target)となるように進化します。

コンパイルエラーが発生する場合は、ランダムデバイスに関わる部分を構造体の内部ではなくグローバルで使用する必要があります。こちらについては、後日グローバルへ移動させたプログラムを追加します。この実装となった理由は、突然変異や交叉に関わる情報は遺伝子(genome)が持っている方が自然だと考えたからです。

このプログラムは、室蘭工業大学計算知能研究室のゼミで使用するために作成しました。改変や応用は自由にして頂いて構いません。使用報告も不要です。

# PSO_Sample

PSO(Particle Swarm Optimization)の簡単なサンプルプログラムです。今回使用したベンチマーク関数はAckley Functionと呼ばれるもので、全ての位置ベクトルが0の時が最適解です。

粒子(particle)1つ1つが、以下の情報を保有しています。

・その粒子のこれまでに探索した点のうち、最も良かった点の位置ベクトル(parsonalBest)
・すべての粒子のこれまでに探索した点のうち、最も良かった点の位置ベクトル(globalBest)
・その粒子が前回動いた速度ベクトル(v)

W,Cp,Cgの数値を弄ると、局所解にハマってしまったり、収束速度が変わったりします。また、目的関数の次元数を増やすと最適解を導くのが困難になります。

基本的に操作する部分は、15行目から19行目にある値だけです。

このプログラムは、室蘭工業大学計算知能研究室のゼミで使用するために作成しました。改変や応用は自由にして頂いて構いません。使用報告も不要です。


# 最後に

不適切なプログラムになっている、またはここがよくわからない、という指摘があれば、twitter:@sakaki_tohruまで連絡をください。