# クローン

## クローンとは

gitにより行える主な作業の1つに、他のユーザーのサーバーでホストされているコードのローカルコピーの作成があります。このコピーを作成するプロセスをクローン作成と呼びます。`git clone`コマンドを使用し、GitHub上にOpen Pixel Artリポジトリのローカルコピーを作成します。

## クローンの作成方法

gitコマンドラインツールには、この作業を行う`clone`というコマンドが用意されています。このコマンドを使用するには、クローンを作成するgitリポジトリのURLを取得する必要があります。

GitHubでは、ホスティングしているリポジトリの[URLを取得する方法に関するドキュメント](https://help.github.com/en/articles/cloning-a-repository)が用意されています。この記事には、クローン作成の全プロセスが詳しく説明されていますが、ここでも説明します。

GitHubから、`https://`で始まり、`.git`で終わるURLを見つけ出します。以下のように表示されるはずです。

```
https://github.com/twilio-labs/open-pixel-project
```

このURLを取得した後、次のように、`git clone`コマンドの後にこのURLを続けて、ターミナルで実行します。

```
git clone https://github.com/twilio-labs/open-pixel-project
```

クローン作成プロセスが開始されます。

## ディレクトリを変更する

リポジトリのクローン作成が完了した後、それらの新しいファイルを開くことができます。そのファイルは、GitHub上に現在あるファイルの正確なコピーです。

クローンが正しく完了したことを確認するには、新しくクローンを作成したプロジェクトの完全なファイルパスが必要です。ディレクトリ変更コマンドの`cd`を入力し、新しいディレクトリに入ります。

```
cd open-pixel-art
```

リストコマンドの`ls`（Windowsでは`dir`）を実行すると、`package.json`や`README.md`などのファイル名のリストが表示されます。

```
ls
```

## 作業ディレクトリを提示する

新しくクローンされたリポジトリをターミナルで開いた後、そのパスを取得する必要があります。現在の作業ディレクトリコマンドの`pwd`を実行し、パスを確認します。

```
pwd
```

このディレクトリをファイルエクスプローラまたはテキストエディタで開くと、Open Pixel Artリポジトリのクローンも表示されます。

## 検証

`pwd`コマンドから取得した、クローンしたリポジトリへのファイルパスをコピーします。右側のフィールドにファイルパスを貼り付けて[`HACK`]を押します。