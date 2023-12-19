# ブランチを作成するまで

各Stepごとに答えを記載します。

## `mainブランチ`をチェックアウトしていることを確認しましょう

今どこのブランチにいるかは、以下のコマンドをターミナルに入力することで確認できます。

```
git branch
```

上記コマンドを入力することで以下のような表示になります。  
![ブランチ一覧を表示](/public/images/lesson/step01/untilCreateBranch01.png)

現在ローカルで持っているブランチ一覧が表示されます。  
他とは異なる色が現在チェックアウトしているブランチになります。  
`*`のマークも現在チェックアウトしているブランチになります。

## `developブランチ`をチェックアウトしましょう

`mainブランチ`から`developブランチ`に切り替えるには、以下のコマンドをターミナルに入力することでブランチを切り替えることができます。

```
git checkout [branch_name]
```

developブランチに切り替えるコマンド
```
git checkout develop
```

上記コマンドを実行したら、以下の画像のように`mainブランチ`から`developブランチ`に色と`*`が移っていることが確認できれば、ブランチの切り替えが成功です。

![developブランチに切り替え](/public/images/lesson/step01/untilCreateBranch02.png)

## `developブランチ`から2つ新しいブランチを作成しましょう。  

`developブランチ`から新しいブランチを作成する際は、以下のコマンドをターミナルに入力します。  
ブランチの作成は1つずつ行います。複数まとめて作成はできないです。

```
git checkout -b [branch_name]
```

developブランチからブランチを作成
```
git checkout -b feature/check-type
```

上記コマンドを実行したら、以下の画像のように新しく`feature/check-typeブランチ`が作成されます。  

![feature/check-typeブランチを作成](/public/images/lesson/step01/untilCreateBranch03.png)

もう1つ作成する必要があります。`developブランチ`にチェックアウトしてから、`feature/add-list-itemブランチ`を作成しましょう。