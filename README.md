# LaTeXテンプレート(和文)
## 概要
- 和文LaTeXテンプレート
- TeX Live 2020対応
- コンパイラはLuaLaTeXもしくはupLaTeXから選択可能
- [日本機械学会](https://www.jsme.or.jp/publish/transact/)指定の書式に概ね準拠している

|タイトル|目次|本文|
|:---:|:---:|:---:|
| <img src="/figure/screenshots/title.png" width="300"> | <img src="/figure/screenshots/contents.png" width="300"> | <img src="/figure/screenshots/body.png" width="300"> |

## テンプレート
- thesis.tex
    - 卒論・修論・博論向け
        - 作成する論文の種別に応じて`thesis.tex`の該当行をコメントアウトしてください  
            ```tex
            % 卒論の場合（修論の場合はmasterの行を有効にする）
            % \newcommand{\thesistype}{doctor}  % 博士論文
            % \newcommand{\thesistype}{master}  % 修士論文
            \newcommand{\thesistype}{bachelor}  % 卒業論文
            ```
- wordstyle.tex
    - MS Word風テンプレート．簡単な報告書作成用．

## 環境構築
### ローカル環境構築
- [TeX Live 2020](http://mirror.aarnet.edu.au/pub/CTAN/systems/texlive/Images/)を導入
- VS Codeの拡張機能[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)を導入
- `$ kanji-config-updmap-sys --ja ms`として，埋め込む和文フォントを設定

### Dockerを使用する場合
- VS CodeのRemote Development機能を使用
- 拡張機能[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)が導入されているので，`Ctrl`+`Alt`+`B`でコンパイルできる
- `thesis.tex`をコンパイルする際は，Windows関連のフォント設定をコメントアウトする必要あり(`wordstyle.tex`はそのままで動作する)

## 備考
- 文献は`.bib`ファイルで管理しています
- `.bib`ファイルに記載の文献情報は[refviewer](https://kujirai.shinyapps.io/refviewer/)より確認することが可能です
- `.bib`ファイルは各種文献管理ソフトや[文献管理スクリプト](https://github.com/sKujirai/reference-bib)より作成することができます
