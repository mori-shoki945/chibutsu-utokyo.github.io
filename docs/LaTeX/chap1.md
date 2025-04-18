# LaTeXの基礎知識
## はじめに
LaTeX は TeX という組版ソフト上で構築されたフリーの文書処理システムであり、TeX 自体は1978年に、LaTeX は1984年に初版が出た古いソフトではあるものの今でも有志によって管理・開発が続けられ、世界中で幅広く使われています。
LaTeX はマークアップ言語と言われるものの一種であり、Wordなどといった WYSIWYG（*What you See Is What You Get*。表示内容が出力内容に一致する）なものと違い、何をしたいのかという**命令**を記述していきます。
<!-- また、LaTeX の文書はどのようなエディタでも（例えば emacs や VSCode）書くことができます。 -->
LaTeX の本体はフリーなソフトウェアであり、どのようなエディタ（例えば emacs や VSCode）であろうとどのようなOS（例えば Mac や Windows）であろうと正しい記法で書かれたtexファイルであれば、最終的な出力結果は同じものが得ることができます。また、理学系の学生としては数式の記述が非常に得意であることもメリットの一つでしょう。
上記のように便利である一方で、2023年現在で LaTeX は未だに開発が進んでいるため注意をしなければいけない点が多くあることや少し複雑な点もあることも事実です。

なお、TeX や LaTeX はそれぞれ「テック」「テフ」や「ラテック」「ラテフ」と読みます。また、TeX・LaTeX のロゴのデザインは決まっています。本書のように組版処理による表記ができない場合には**TeX**、**LaTeX**と書くルールになっています。

本演習におけるサンプルファイルは
[ここ](https://github.com/chibutsu-utokyo/chibutsu-utokyo.github.io/tree/main/docs/LaTeX/sample)
に置いてあります。

## 日本語のできるLaTeX
2023年現在で、日本語を正しく扱える LaTeX は以下の3つです。

* **pLaTeX**
    * 日本語のできるLaTeX
* **upLaTeX**
    * Unicode化されたpLaTeX
* **LuaLaTeX**
    * 高機能な新しいLaTeX。残りの2つより遅い
    
!!!note
    ここで言う「日本語のできるLaTeX」とは正確には「日本語組版を実現できるLaTeX」を指します。
    例えばXeLaTeXは現在でも日本語を扱うことはできますが、日本語の組版を完全に実現することはできていません。

上記の3つのLaTeXのうち、pLaTeXとupLaTeX（**(u)pLaTeX**と表記します）は親戚のような関係であり、LuaLaTeXはこれらとは少し異なったLaTeXになっています。
その都合上、どのLaTeXを使うかによって少し書き方が異なる点や注意しなければいけない点が出てきます。

特に理由のない場合にはupLaTeXかLuaLaTeXのいずれかを使えば良いと思います。

## LaTeX の利用方法
現在では LaTeX を利用する方法がいくつかあります。簡単なメリット・デメリットと共にいくつか例をあげておきたいと思います。

* **ローカルに環境を整える**
    * 自分のPC上に LaTeX が使える環境を作る方法
    * オフライン環境でも文書作成ができるが慣れていないと少し難しい[^1]
* **[OverLeaf](https://www.overleaf.com/)**を使う
    * クラウド上で使えるサービス
    * 複数人執筆や文書の変更履歴を確認できる
    * pLaTeX や upLaTeX の利用に*魔法の言葉*が必要
* **[Cloud LaTeX](https://cloudlatex.io/ja)**を使う
    * クラウド上で使えるサービス
    * 日本の企業が提供しているため利用しやすい
    * 利用可能な容量に制限がある

本演習ではCloud LaTeXを利用することにします。

[^1]: 参考：[TeX入手法-TeXWiki](https://texwiki.texjp.org/?TeX%E5%85%A5%E6%89%8B%E6%B3%95)
