
- ユーザ名を登録する
- リモートリポジトリ`https://github.com/uzipon-wireless/git_study.git`を`origin`を紐付ける
- 


```bash
$ git config --global user.name uzipon-wireless
$ git remote add origin https://github.com/uzipon-wireless/git_study.git
$ git push -u origin master
```

```bash
$ git branch
* master
$ git remote
$ git remote -v
$ git rev-parse --abbrev-ref HEAD 
master
$ git remote -v
$ git branch
* master
$ git remote add origin https://github.com/uzipon-wireless/vscode.git
$ git remote -v
origin	https://github.com/uzipon-wireless/vscode.git (fetch)
origin	https://github.com/uzipon-wireless/vscode.git (push)
$ git branch -M main
$ git branch
* main
$ git push -u origin main
Username for 'https://github.com': uzipon-wireless
Password for 'https://uzipon-wireless@github.com': 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 832 bytes | 416.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/uzipon-wireless/vscode.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.

```



## 参考
githubでrepoを作成すると表示されるチュートリアル

### create a new repository on the command line
```bash
echo "# vscode" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/uzipon-wireless/vscode.git
git push -u origin main
```

### push an existing repository from the command line
```bash
git remote add origin https://github.com/uzipon-wireless/vscode.git
git branch -M main
git push -u origin main
```

以上