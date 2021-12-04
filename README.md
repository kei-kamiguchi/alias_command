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
alias rb30="cd ~/programing/ruby/version3.0/test"
alias py38="cd ~/programing/python/version3.8/test"


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

# Homebrew
export PATH="/opt/homebrew/bin:$PATH"

# Ruby
eval "$(rbenv init -)"

# PostgreSQL
export PATH="/opt/homebrew/opt/postgresql@13/bin:$PATH"

# nvm
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm

# Python
eval "$(pyenv init --path)"

# PHP
export PATH="/usr/local/opt/bison/bin:$PATH"
export PATH="/usr/local/opt/libxml2/bin:$PATH"
export PATH="/usr/local/opt/bzip2/bin:$PATH"
export PATH="/usr/local/opt/curl/bin:$PATH"
export PATH="/usr/local/opt/libiconv/bin:$PATH"
export PATH="/usr/local/opt/krb5/bin:$PATH"
export PATH="/usr/local/opt/openssl@1.1/bin:$PATH"
export PATH="/usr/local/opt/icu4c/bin:$PATH"
export PATH="/opt/homebrew/opt/tidy-html5/lib:$PATH"
export PKG_CONFIG_PATH="/opt/homebrew/opt/libzip/lib/pkgconfig:$PKG_CONFIG_PATH"
export PKG_CONFIG_PATH="/opt/homebrew/opt/libjpeg/lib/pkgconfig:$PKG_CONFIG_PATH"
export PKG_CONFIG_PATH="/opt/homebrew/opt/libpng/lib/pkgconfig:$PKG_CONFIG_PATH"
export PKG_CONFIG_PATH="/opt/homebrew/opt/oniguruma/lib/pkgconfig:$PKG_CONFIG_PATH"
export PKG_CONFIG_PATH="/usr/local/opt/krb5/lib/pkgconfig:$PKG_CONFIG_PATH"
export PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig:$PKG_CONFIG_PATH"
export PKG_CONFIG_PATH="/usr/local/opt/icu4c/lib/pkgconfig:$PKG_CONFIG_PATH"
export PHP_RPATHS="/usr/local/opt/zlib/lib /usr/local/opt/bzip2/lib /usr/local/opt/curl/lib /usr/local/opt/libiconv/lib /usr/local/opt/libedit/lib"
export PHP_BUILD_CONFIGURE_OPTS="--with-zlib-dir=/usr/local/opt/zlib --with-bz2=/usr/local/opt/bzip2 --with-curl=/usr/local/opt/curl --with-iconv=/usr/local/opt/libiconv --with-libedit=/usr/local/opt/libedit"
```
