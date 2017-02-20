## 2017/02/20
### importファイルのまとめ方の注意点
importするファイルを親要素でネストさせるのはよくない。
```
// ダメな例
#parent {
    @import _main.scss
    @import _sub.scss
    @import _others.scss
    ...
}
```