https://stackoverflow.com/questions/13363553/git-error-host-key-verification-failed-when-connecting-to-remote-repository

```shell
ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts
```

### 拉取远程分支（本地无此分支）

```shell
git checkout -b dev(本地分支名称) origin/dev(远程分支名称)
```
