#SourceTree for Mac 使い方
---
皆さんはGitの基本的な使い方は理解していると思いますが、今回は`SourceTree`を使ってGitを使っていきたいと思います。もし、Gitで使う用語などがわからない場合は[こちら](https://github.com/techlogics/Git_Document/blob/master/grammer.md)からまずは基礎をお勉強してからこのドキュメントを見てくれると嬉しいです。まずは`SourceTree`を[こちら](https://www.atlassian.com/ja/software/sourcetree/overview)からダウンロードしてインストールしてください。

## リポジトリの作成
![](https://www.evernote.com/shard/s324/sh/2c91ebee-e59f-41e3-afce-137aa94a9eb2/7384eae35f7f4e56ee0ca719b59eb509/deep/0/SourceTree.png)

矢印のボタンを押すとアカウント、所有者、リポジトリの名前、説明、タイプを入力してリポジトリを作成します。

そうするとリポジトリ一覧に先ほど作成したリポジトリが現れるので開いてあげましょう。開くと次のような画面になると思います。
![](https://www.evernote.com/shard/s324/sh/c06b8223-cd74-4607-b63a-7290921b44ee/40938b6ba19a1e75658f8724500a86dc/deep/0/MyFirstRepository-(Git).png)

## バージョン管理
では早速新しくファイルを作ってGitで管理してみましょう。ファイル名は`test.txt`とします。中身を適当に編集してみます。
![](https://www.evernote.com/shard/s324/sh/0ecea076-607e-4645-889f-8823cb31ee23/946870f447e26e78dc4e9d3f00831d21/deep/0/test.txt---Git_Document.png)

SourceTreeに移ってコミットをしてみましょう。
![](https://www.evernote.com/shard/s324/sh/605a79a9-631e-4a7a-a489-ccd6469341bc/348d7d80907a2870c039d70eb841f1ad/deep/0/MyFirstRepository-(Git).png)

現在ファイルはコミットする準備ができていない状態(ステージされていない状態)でこれをステージングしてあげる必要があります。下の`unstaged files`からステージングしたいファイルを選択してください。

それではいよいよコミットです。
![](https://www.evernote.com/shard/s324/sh/bb13e899-81ec-4535-96bf-644279625d7e/60ed1c3c3fcb622b7441e27fd6063376/deep/0/MyFirstRepository-(Git).png)

矢印のコミットボタンを押してコミットしましょう。
するとコミットメッセージを入力するように言われますのでコミットメッセージを書きましょう。コミットメッセージの書き方は[こちら](http://qiita.com/itosho/items/9565c6ad2ffc24c09364)の記事が参考になります。
コミットメッセージを書いたらコミットを押してください。

終わるとこのように画面上の`Push`のボタンにバッジがついたと思います。次はこれをサーバーにプッシュしたい思います。プッシュボタンを押すとリポジトリとブランチを選択する画面が現れますがデフォルトの`master`で問題ないのでそのままプッシュしましょう。プッシュが終わったらGithubに行って自分のプッシュを確認してみましょう。

## コンフリクトの対処方法
```git
<<<<<<< HEAD
コンフリクト
=======
コンフリクトその②
>>>>>>> FETCH_HEAD
```
の`<<<<<<< HEAD`から`=======`までが自分の編集した部分で`=======`から`>>>>>>> FETCH_HEAD`が相手の編集した部分になります。これを編集して再度コミットしてあげることで解消することができます。