# robosys_new
2021ロボットシステム学の課題１で作成したものです。

## 動作環境

・Rasberry Pi4 Model　B

・OS:ubuntu 20.04 server

## 使用したもの

・Rasberry Pi4 Model　B

・LED ×　1

・抵抗　200Ω　×　1

・ブレッドボード　×　１

・ジャンパー線　× 6


## 配線図

![配線図](https://user-images.githubusercontent.com/95580448/146232864-489d3742-2dac-43bd-8d5e-825c952cef02.jpg)

## 使用方法

・インストール

```sh
$ git clone https://github.com/NatsuTsuchida/robosys.git
$ cd robosys/myled
$ make
```

・権限

```sh
$sudo insmod myled.ko
$sudu chmod 666 /dev/myled0
```

・アンインストール

```sh
$sudo rmmod myled
$make ckean
```

・LEDをつける

```sh
$echo 1 > /dev/myled0
```

・LED を消す
```sh
$echo 0 > /dev/myled0
```
## 実行

https://youtu.be/-Do5iTJT3wM

## ライセンス

[GNU General Public License v3.0](https://github.com/NatsuTsuchida/robosys/blob/main/COPYING)
