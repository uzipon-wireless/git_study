
- ユーザ名を登録する
- リモートリポジトリ`https://github.com/uzipon-wireless/git_study.git`を`origin`を紐付ける
- 


```bash
$ git config --global user.name uzipon-wireless
$ git remote add origin https://github.com/uzipon-wireless/git_study.git
$ git push -u origin master
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