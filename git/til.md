## 2017/02/22  
### Gitで更新からpushするまでのコマンドを覚える  
とりあえず記憶だけで書いてみる
```
// 変更したファイルを登録  
git add all

// コミット
git commit -m "コメント"

// リモートへプッシュ
git push origin master
```

__答え合わせ__  
だいたい合ってた。  
間違ったのは下記  
`git add all` ==> `git add --all` もしくは `git add --a`  
  
もっといろんなコマンドがあるので、困ったら素直に[Qitaの記事](http://qiita.com/konweb/items/621722f67fdd8f86a017)とか見よう。
