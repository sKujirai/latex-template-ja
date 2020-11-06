# LaTeXテンプレート(和文)
## 概要
- 和文LaTeXテンプレート
- TeX Live 2020対応
- コンパイラはLuaLaTeXもしくはupLaTeXから選択可能
- [日本機械学会](https://www.jsme.or.jp/publish/transact/)指定の書式に概ね準拠している

## テンプレート
- thesis.tex
    - 卒論・修論・博論向け
- wordstyle.tex
    - MS Word風テンプレート．簡単な報告書作成用．

## 環境構築
### ローカル環境構築
- [TeX Live 2020](http://mirror.aarnet.edu.au/pub/CTAN/systems/texlive/Images/)を導入
- VS Codeの拡張機能[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)を導入
- `$ kanji-config-updmap-sys --ja ms`として，埋め込む和文フォントを設定

### Dockerを使用する場合
- VS CodeのRemote Development機能を使用
- `wordstyle.tex`のみ動作確認済み．`thesis.tex`をコンパイルする際は，追加のパッケージのインストールが必要
