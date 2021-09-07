# PostScriptでスライド作成

## 仕様

- \#〜\###はmdと同様
- \[M]で明朝、\[G]でゴシック
- \<r,g,b> で以後その行はrgb色

## 利用

```sh
    gs -g1920x1080 -sDEVICE=png16m -dTextAlphaBits=4 -r125 -sOutputFile=out/slide%d.png ./read_md.ps <text.md
```
でスライド画像出力