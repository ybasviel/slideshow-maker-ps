# PostScriptでスライド作成

## 仕様

- \#〜\###はmdと同様
- \#で新ページ
- \\[M]で明朝、\\[G]でゴシック
- \\<r,g,b> で以後その行はrgb色

## 利用

```shell
gs -q -dNOSAFER -g1920x1080 -sDEVICE=png16m -dTextAlphaBits=4 -r125 -sOutputFile=out/slide%d.png ./make-slide.ps
```
でスライド画像出力


```shell
gs -q -g1920x1080 -r125 -dNOSAFER ./make-slide.ps
```
で発表者モード