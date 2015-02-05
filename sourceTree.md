#SourceTree for Mac 使い方
---
皆さんはGitの基本的な使い方は理解していると思いますが、今回は`SourceTree`を使ってGitを使っていきたいと思います。もし、Gitで使う用語などがわからない場合は[こちら](https://github.com/techlogics/Git_Document/blob/master/grammer.md)からまずは基礎をお勉強してからこのドキュメントを見てくれると嬉しいです。まずは`SourceTree`を[こちら](https://www.atlassian.com/ja/software/sourcetree/overview)からダウンロードしてインストールしてください。

リポジトリの作成
-

バージョン管理
-

コンフリクトの対処方法
-

```git
<<<<<<< HEAD
コンフリクト
=======
コンフリクトその②
>>>>>>> FETCH_HEAD
```
の`<<<<<<< HEAD`から`=======`までが自分の編集した部分で`=======`から`>>>>>>> FETCH_HEAD`が相手の編集した部分になります。これを編集して再度コミットしてあげることで解消することができます。