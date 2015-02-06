#SourceTree for Mac 使い方
---
皆さんはGitの基本的な使い方は理解していると思いますが、今回は`SourceTree`を使ってGitを使っていきたいと思います。もし、Gitで使う用語などがわからない場合は[こちら](https://github.com/techlogics/Git_Document/blob/master/grammer.md)からまずは基礎をお勉強してからこのドキュメントを見てくれると嬉しいです。まずは`SourceTree`を[こちら](https://www.atlassian.com/ja/software/sourcetree/overview)からダウンロードしてインストールしてください。

## リポジトリの作成
![](https://www.evernote.com/shard/s324/sh/2c91ebee-e59f-41e3-afce-137aa94a9eb2/7384eae35f7f4e56ee0ca719b59eb509/deep/0/SourceTree.png)

矢印のボタンを押すとアカウント、所有者、リポジトリの名前、説明、タイプを入力してリポジトリを作成します。

そうするとリポジトリ一覧に先ほど作成したリポジトリが現れるので開いてあげましょう。開くと次のような画面になると思います。
![](https://www.evernote.com/shard/s324/sh/c06b8223-cd74-4607-b63a-7290921b44ee/40938b6ba19a1e75658f8724500a86dc/deep/0/MyFirstRepository-(Git).png)

## バージョン管理

## コンフリクトの対処方法
```git
<<<<<<< HEAD
コンフリクト
=======
コンフリクトその②
>>>>>>> FETCH_HEAD
```
の`<<<<<<< HEAD`から`=======`までが自分の編集した部分で`=======`から`>>>>>>> FETCH_HEAD`が相手の編集した部分になります。これを編集して再度コミットしてあげることで解消することができます。