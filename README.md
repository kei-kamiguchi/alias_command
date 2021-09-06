# エイリアスコマンドを使ってコマンド入力を簡略化する
zshの設定ファイル`~/.zshrc`に以下のコードを貼り付けることで、コマンドの入力が超楽。
コマンド忘れてもすぐに参照できる。`cd`は自身の環境に合わせて定義すればOK。
```zsh
# shell
alias brc="vi ~/.bashrc"
alias bpro="vi ~/.bash_profile"
alias sbrc="source ~/.bashrc"
alias sbpro="source ~/.bash_profile"
alias zrc="vi ~/.zshrc"
alias zpro="vi ~/.zprofile"
alias szrc="source ~/.zshrc"
alias szpro="source ~/.zprofile"
alias cred="EDITOR=vim rails credentials:edit"

# git
alias gita.="git add ."
alias gita="git add"
alias gitbr="git branch"
alias gitbrd="git branch -D"
alias gitpsm="git push origin master"
alias gitplm="git pull origin master"
alias gitps="git push origin"
alias gitpl="git pull origin"
alias gitst="git status"
alias gitchob="git checkout -b"
alias gitcho="git checkout"
alias gitrms="git remote set-url origin"
alias gitrma="git remote add origin"
alias gitcl="git clone"
alias gitclb="git clone -b"
alias gitrmv="git remote -v"
alias gitcom="git commit"
alias gitcomm="git commit -m"
alias gitcho.="git checkout ."
alias gitc="git clean -df ."
alias gitlogo="git log --oneline"
alias gitrsh="git reset --hard"
alias gitrss="git reset --soft"
alias gitauto="git add . && git commit -m 'auto commit' && git push origin master"
alias gitautof="git add . && git commit -m 'auto commit' && git push origin master -f"
alias gitst="git stash -u"
alias gitstap="git stash apply"
alias gitstl="git stash list"

# cd

# rails
alias rs="rails s"
alias rc="rails c"
alias rr="rails routes"
alias dbc="rails db:create"
alias dbm="rails db:migrate"
alias dbcm="rails db:create && rails db:migrate"
alias dbd="rails db:drop"
alias dbr="rails db:reset"
alias dbs="rails db:seed"
alias dbb="rails db:rollback"
alias dbmr="rails db:migrate:reset"
alias dbset="rails db:setup"

# yarn
alias yic="yarn install --check-files"

# rspec
alias brs="bundle exec rspec"
alias brsf="bundle exec rspec spec/ --fail-fast"

# deploy
alias capd="cap production deploy"
```
