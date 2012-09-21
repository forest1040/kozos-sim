#kozos-sim
([KOZOS](http://kozos.jp/kozos/index.html "KOZOSプロジェクト"))の組込み用のオープンソースOSであるKOZOSをシミュレータ環境で動作させるためのパッチファイルです。
シミュレータ環境は、gdbのCPUエミュレーション機能を使用します。

##参考URL
((http://kozos.jp/kozos/h8_sim_01.html "(シミュレータ編第１回)とりあえず動かしてみた"))

##手順
* gdb-7.2.tar.gzをダウンロードして展開
* 以下の3つのパッチを当てる。
    * Makefile.in.patch
    * Makefile.patch (configure実行済みの場合)
    * compile.c.patch

* 以下の2つのファイルを「gdb/sim/h8300/」以下にコピーする
    * device.c
    * serial.c

