## 2017/03/10  
### Jekyllをインストールした時にOperation not permittedとエラーが出た件
```
$ gem install jekyll
```
`sudo` をつけてみてもダメ。  
El Capitan以上だとセキュリティ機能 `Rootless` なるものが追加されており、rootユーザーであってもアクセス制限が掛けられるそうです。  
  
- __解決策__  
Macを再起動して、起動時に「Command + R」を押し続けてリカバリーモードで起動する  
ターミナルを起動して次のコマンドを実行  
```
$ csrutil status //状態確認
$ csrutil disable  //無効化
```
これでアクセス制限が無効化されインストール可能に。