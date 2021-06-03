# Git チュートリアル

## Git とは？

- ファイルのバージョン管理

  - 新しいバージョンを登録するときに、差分を確認する

  - 新しいバージョンを登録するときに、誰がいつ何のために変更したか記録を残す

  - 古いバージョンに戻す

  - 二つのバージョン間の差分を確認する

    

- 多人数でファイルを共有しながらバージョン管理

  - 他の人が変更した内容も取り込める
  - 自分が変更した内容を他の人も利用できる



## Git を使ってみる

git で新しいバージョンを登録するときは、誰が登録したのか記録されるので、まず自分の名前とメールアドレスを git に設定する。

```shell
git config --global user.name "Komura Takaaki"
git config --global user.email komura@example.com
```



バージョン管理されているこのファイルを取得してみる。

```shell
git clone https://github.com/emon/git-tutorial.git
cd git-tutorial
```

どんなファイルが入っているか確認する。

```shell
ls -l
```

これまでのバージョンの履歴を確認する。

```shell
git log
```



