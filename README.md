# プログラミング用フォント Ricty Diminished w/ Powerline patched

Ricty Diminished (リクティ・ディミニッシュト) は [Ricty](https://github.com/yascentur/Ricty) の姉妹フォントであり、[Inconsolata](http://levien.com/type/myfonts/inconsolata.html) と [Migu 1M](http://mix-mplus-ipa.sourceforge.jp/) ではなく、[Inconsolata](http://levien.com/type/myfonts/inconsolata.html) と [Circle M+ 1m](http://mix-mplus-ipa.sourceforge.jp/) を Ricty 生成スクリプトで合成したフォントです。
IPA ゴシックのグリフを含まないため、使用可能な漢字グリフの数が少ない代わり、[SIL Open Font License](http://scripts.sil.org/ofl) の下で配布が可能です。

# 特徴

* ラテン文字には Raph Levien 氏の Inconsolata が適用されます。
* それ以外の文字には Circle M+ 1m が適用されます。美しい M+ と itouhiro 氏が改良された視認性の高い日本語文字 (半濁音など) が使用できます。
* 半角文字と全角文字の横幅の比が 1:2 に調整されています。
* 全角スペースが可視化されます。
* いくつかの全角グリフが対応する半角グリフと差別化されています。
* en ダッシュ、em ダッシュが破断線のようになります (LaTeX での入力ミス防止のため)。
* **0x2b60-0x2b64, 0x2b80-0x2b84にPowerline用のグリフが埋め込まれたバージョン(\*-Powerline.ttf)を追加で収録**

# ライセンス

* Ricty Diminished は [SIL Open Font License (OFL) Version 1.1](http://scripts.sil.org/ofl) に従うものとします。

# バージョン

## Version 3.2.4-Powerline (15 Jan. 2016)

* Ricty Diminished Version 3.2.4ベース
* [powerline/fontpatcher](https://github.com/powerline/fontpatcher.git)をsubmoduleとして追加
* powerline/fontpatcherを以下のように実行し、Powerlineグリフ埋め込みバージョンを作成
```
$ ls RictyDiminished*.ttf | grep -v Powerline | xargs fontpatcher/scripts/powerline-fontpatcher
```

## Version 3.2.4-Powerline (11 May. 2015)

* Ricty Diminished Version 3.2.4ベース
* [vim-powerline](https://github.com/Lokaltog/vim-powerline.git)をsubmoduleとして追加
* vim-powerlineに付属のfontpatcherをfontforge-20110225で以下のように実行し、Powerlineグリフ埋め込みバージョンを作成
```
$ find . -name '*.ttf' -exec fontforge -script vim-powerline/fontpatcher/fontpatcher {} \;
```

## Version 3.2.4 (7 Dec. 2014)

* [Ricty 生成スクリプト Version 3.2.4](https://github.com/yascentur/Ricty/tree/3.2.4)
* Inconsolata Version 001.010
* Circle M+ 1m Version 1.056

## Version 3.2.3 (4 May 2014)

* [Ricty 生成スクリプト Version 3.2.3](https://github.com/yascentur/Ricty/tree/3.2.3)
* Inconsolata Version 001.010
* Circle M+ 1m Version 1.056

## Version 3.2.2 (9 June 2013)

* [Ricty 生成スクリプト Version 3.2.2](https://github.com/yascentur/Ricty/tree/3.2.2)
* Inconsolata Version 001.010
* Circle M+ 1m Version 1.055

## Version 3.2.1 (6 Nov. 2012)

* [Ricty 生成スクリプト Version 3.2.1](https://github.com/yascentur/Ricty/tree/3.2.1)
* Inconsolata Version 001.010
* Circle M+ 1m Version 1.052

# 作者連絡先

[遊佐泰紀 (Yasunori Yusa)](http://save.sys.t.u-tokyo.ac.jp/~yusa/index.html.ja)
