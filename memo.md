## 2017/3/3

### 過去のgit commitのauthorを変更する

- git rebaseで対象のcommitをすべてeditする
- git commit --amend --author="user.name <user.email>"

```
$ git rebase -i <commit-hash>
<<
pick hoge
pick piyo
>>
edit hoge
edit piyo
$ git commit --amend --author="hhashimoto <hoge@piyo.com>"
$ git rebase --continue
```

ref. [http://stackoverflow.com/questions/3042437/change-commit-author-at-one-specific-commit](http://stackoverflow.com/questions/3042437/change-commit-author-at-one-specific-commit)
