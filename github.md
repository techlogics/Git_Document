#Github for Mac 使い方
---
皆さんはGitの基本的な使い方は理解していると思いますが、今回はGithub公式のクライアントを使ってGitを使っていきたいと思います。もし、Gitで使う用語などがわからない場合は[こちら](https://github.com/techlogics/Git_Document/blob/master/grammer.md)からまずは基礎をお勉強してからこのドキュメントを見てくれると嬉しいです。まずはGithubのクライアントを[Macの方はこちら](https://mac.github.com/) / [Windowsの方はこちら](https://windows.github.com/)からダウンロードしてインストールしてください。

リポジトリの作成
-
設定済ませて起動するとこんな感じの画面になると思います。
![](https://www.evernote.com/shard/s324/sh/95aaac3a-653c-40a1-b83e-ae8afb5dac03/d196f065b3e76426e10f5140ed39360e/res/9393d8f2-4751-42c3-94c0-1ad5700d506e/skitch.png)

では実際に`Repository`を作っていきましょう。左上のプラスボタンからリポジトリを作ります。
![](https://www.evernote.com/shard/s324/sh/1b8f8939-a629-445d-8c5a-efbc5c4650cb/fefaf54d106191f5be743bd19a6d7aa9/res/52423c1d-c3a7-4bfb-b3d0-a7c8763f85c4/skitch.png)

次に右上の`Publish`ボタンからリポジトリをGithubにプッシュしたいと思います。
![](https://www.evernote.com/shard/s324/sh/6010c73c-52c6-474e-84fd-3aec8fdb4be5/9f426a0f4ccd3c6a7305d9e9ae006eb1/res/4d47c1c0-c340-479d-8826-d8035eaebd36/skitch.png)
これで無事にGithubにリポジトリが追加されたと思います。

バージョン管理
-
バージョン管理したいファイルを先ほど設定したローカルのパスにD&D(ドロップ&ドラッグ)してください。
![](https://www.evernote.com/shard/s324/sh/bf34050d-b970-459e-9c42-802af78f1982/cfef048ff07eafd3b5305fe9cf5f987e/deep/0/MyFirstRepository.png)

そしたらGithub for Macを開いてみましょう。先ほど追加したファイルが表示されていると思います。ファイルの変更箇所などが表示されます。ではコミットメッセージを入力してコミットしてみましょう。
![](https://www.evernote.com/shard/s324/sh/f88efc64-f422-4ef6-9244-7e8c145b12dd/41afeba62f8dbd80c9490c1094fb8852/deep/0/tkcfjips-MyFirstRepository.png)

では、コミットができたので次はGithubにプッシュしてみましょう。右上のボタンでプッシュします。ちなみにコミットとプッシュを同時にやりたければ、Commitボタンの左のボタンをクリックすることでコミットとプッシュを同時にしてくれるようになります。
![](https://www.evernote.com/shard/s324/sh/059d14d4-4b07-4f0f-b753-baacc2561cbd/e49c9deae2aa28ddf37c42cc2476c0b3/deep/0/tkcfjips-MyFirstRepository.png)

[github.com](github.com)に行ってうまくいっているか確認してみましょう。うまくいっていればこのようになっているはずです。
![](https://www.evernote.com/shard/s324/sh/af6f9d4d-7264-4a53-874b-4cba0df67d99/96692efdff38976a2a76d69cb6fd8781/deep/0/tkcfjips-MyFirstRepository-and-tkcfjips-MyFirstRepository.png)

コンフリクトの対処方法
-
これがコンフリクトが起きたときの画面です。
![](https://www.evernote.com/shard/s324/sh/b738d51e-bd7c-4761-9fed-77aa3c15bcc5/3cf133c2b280ab159ee8c5f80e142408/deep/0/tkcfjips-MyFirstRepository.png)

```git
<<<<<<< HEAD
コンフリクト
=======
コンフリクトその②
>>>>>>> FETCH_HEAD
```
の`<<<<<<< HEAD`から`=======`までが自分の編集した部分で`=======`から`>>>>>>> FETCH_HEAD`が相手の編集した部分になります。これを編集して再度コミットしてあげることで解消することができます。
