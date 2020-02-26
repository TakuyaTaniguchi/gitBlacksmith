# gitBlacksmith

## コミットコメントを間違えた
```
git commit --amend
```

## addを取り消したい。
git reset HEAD {./}

## 間違えてpushした...
履歴を削除せずに直前のデータをローカルに保存し、再度pushする方法がベター
### コミットIDを取得

```
git log
/*
commit ee89100ff5b26bf97113b14851e3d48e2b7f0c4c (HEAD -> master, origin/master)
Author: TakuyaTaniguchi
Date:   Wed Feb 26 11:49:19 2020 +0900
*/
```

### コミットの取り消し

```
git revert <commit id>
```

## ブランチの分岐
Vscodeから作成もしくは

```
 git branch {branchname}
```

### 一覧の取得
```
git branch
```

### push

```
git push {branchname} 
or
git push origin HEAD
```