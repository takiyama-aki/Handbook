# VSCodeでgithubを使う
## ローカルリポジトリ
```
$ git init
```
上記のコードでローカルリポジトリを初期化.
".git"という隠しフォルダがローカルリポジトリとなる。

サイドバーのソース管理(^+shift+G)に移動する。
変更のあるファイル名の右側にある"+"をクリックしステージングを行う。

"メッセージ"というところにコメントを記入し、"✓"でローカルリポジトリにコミットする。

## Githubと連携
Githubにて新しいリポジトリを作成しておく。

ターミナル上で
```
$ git remote add origin [リポジトリのURL]
```

を実行し、ローカルリポジトリと作成したリモートリポジトリを紐づける。
```
$ git branch -M main
```
上記のコマンドで"main"というブランチを作成。
```
$ git push -u origin main
```
を実行し、"main"というブランチに対するプッシュ操作を行う。