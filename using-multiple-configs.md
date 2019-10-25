# gitconfig

ref: https://qiita.com/Ancient_Scapes/items/64f239f89d25a3b9f520

## ~/.gitconfig

```
省略

# workフォルダの時会社用gitアカウントに切り替え
[includeIf "gitdir:~/git-work/"]
  path = ~/.gitconfig-work

# otherフォルダの時は個人用アカウントを使用する
[includeIf "gitdir:~/git-personal/"]
  path = ~/.gitconfig-personal
```

## ~/.gitconfig-work
```
[user]
  email = me@work.com
  name = me
```

## ~/.gitconfig-personal
```
[user]
  email = me@personal.com
  name = me
```

# ~/.ssh/config
ref: https://qiita.com/wonder_zone/items/413abaa45b2d29fd26d6#sshconfig%E3%81%AE%E5%86%85%E5%AE%B9%E4%BE%8B

```
# git-work
Host git-work
  User git
  HostName work.com
  IdentityFile ~/.ssh/id_rsa
  TCPKeepAlive yes
  IdentitiesOnly yes

# git-personal
Host git-personal
  User git
  HostName github.com
  IdentityFile ~/.ssh/github_sub_id_rsa
  TCPKeepAlive yes
  IdentitiesOnly yes
```

# Privacy
Enable "Keep my email addresses private" on github.com if you want to keep your email address private. 

ref: https://kiliware.hateblo.jp/entry/2019/04/30/210000
