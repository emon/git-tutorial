# Git チュートリアル

## Git とは？

- ファイルの版管理

  - 新しい版を登録するときに、差分を確認する

  - 新しい版を登録するときに、誰がいつ何のために変更したか記録を残す

  - 古い版に戻す

  - 二つの版の間の違い(差分)を確認する



- 多人数でファイルを共有しながら版管理

  - 他の人が変更した内容も取り込める
  - 自分が変更した内容を他の人も利用できる



## Git を使ってみる

Raspberry Pi には初期状態で `git` コマンドがインストールされている。Windows や macOS で `git` コマンドがインストールされていない場合は https://git-scm.com/downloads からインストールする。

git で版を登録するときは、誰が操作したのか記録するので、まず、自分の名前とメールアドレスを git に設定する。

```shell
git config --global user.name "Komura Takaaki"
git config --global user.email komura@example.com
```



自分のファイルを `git` で管理し始める前に、既に版管理されているファイルを取得して `git` での版管理の様子を確認してみる。
今読んでいるこのページも `git` で版管理しているので、この内容を例として見てみる。

```shell
git clone https://github.com/emon/git-tutorial.git
cd git-tutorial
```

どんなファイルが入っているか確認する。

```shell
ls -l
```

これまでの版の履歴を確認する。

```shell
git log
```



