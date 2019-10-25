
https://qiita.com/Ancient_Scapes/items/64f239f89d25a3b9f520

~/.gitconfig
省略

# workフォルダの時会社用gitアカウントに切り替え
[includeIf "gitdir:~/project/work/"]
  path = ~/.gitconfig-work

# otherフォルダの時は個人用アカウントを使用する
[includeIf "gitdir:~/project/other/"]
  path = ~/.gitconfig-other

~/.gitconfig-work
[user]
  email = name@work.com
  name = name

~/.gitconfig-other
[user]
  email = name@personal.com
  name = name

Enable "Keep my email addresses private" on github.com if you want to keep your email address private. 
