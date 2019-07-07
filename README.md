# 『30日でできる！ OS自作入門』 for macOS
- [30日でできる！ OS自作入門](https://amzn.to/2JqkIWy)の開発環境をmacOSでも扱えるようにします。

## 動作環境

以下の環境で動作確認を行っています。

- OS
	- macOS Mojave 10.14.5

```bash
$ sw_vers
ProductName:    Mac OS X
ProductVersion: 10.14.5
BuildVersion:   18F132
```

## 環境構築手順

### 1. このレポジトリをclone

```bash
$ git git@github.com:emono/30nichideosjisaku.git
```

### 2. qemuをインストール

```bash
# Homebrewでインストール
$ brew install qemu

# バージョンを確認 (現時点でバージョンは`4.0.0`)
$ qemu-system-i386 -version
QEMU emulator version 4.0.0
Copyright (c) 2003-2019 Fabrice Bellard and the QEMU Project developers
```

### 3. 確認

```bash
$ cd 30nichideosjisaku/01_day/helloos0
$ make run
```

実行して以下のように表示されていれば成功です。

![image](https://github.com/sandai/30nichideosjisaku/raw/master/bin/img/qemu.png)

## URL

- [「30日でできる！ OS自作入門」のサポートページ](http://hrb.osask.jp/)
	- 公式サポートサイト
- [tolsetOSX](http://shrimp.marokun.net/osakkie/wiki/tolsetOSX/)
	- Mac版のtolset配布ページ
- [0xED](http://www.suavetech.com/0xed/0xed.html)
	- バイナリエディタ配布サイト
	
