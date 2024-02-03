## スタイルファイルの準備

1.  biblatexフォルダ内のjsr.bbx、jsr.cbx、jsr.dbxの3つのファイルを、\$TEXMFLOCAL/tex/latex/biblatex-jsrの中に配置する（biblatex-jsrフォルダは自分で作成）。

\$TEXMFLOCALは、terminalで以下のコマンドを実行することで確認できる。

```         
kpsewhich -var-value TEXMFLOCAL
```

2.  terminalで以下のコマンドを実行する。

```         
mktexlsr
```

## 文献スタイルの指定

quartoの場合、yamlの`cite-method`と`biblatexoptions`を以下のように指定。

```{yaml}
cite-method: biblatex
biblatexoptions: [backend=biber, style=jpa, sorting=nyt]
```

## 付記

本スタイルファイルはbiblatex-jpaをもとに作成されています。biblatex-jpaは以下のリポジトリより入手することができます。

[https://github.com/sbtseiji/biblatex-jpa](https://github.com/sbtseiji/biblatex-jpa)
