Spatio-Temporal Databases Labaratory home page

Setting ruby by rbenv
------------------------
ruby version is now managed by rbenv. So after clone this, if environment doesn't use rbenv, then do this.

1. cd $HOME
2. sudo apt-get remove ruby
3. sudo apt-get update 
4. sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
5. git clone https://github.com/rbenv/rbenv.git ~/.rbenv
6. echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
7. echo 'eval "$(rbenv init -)"' >> ~/.bashrc
8. exec $SHELL
9. git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
10. echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
11. exec $SHELL
12. rbenv install 2.3.1
13. rbenv global 2.3.1
14. ruby -v

  Reference for upper steps : 
  https://stackoverflow.com/questions/37720892/you-dont-have-write-permissions-for-the-var-lib-gems-2-3-0-directory

Setting environment
------------------------
From now on, I will describe how to set environment for jekyll.
Reference is here : https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/

Here are setting steps.

1. bundle update
2. sudo apt install nodejs
3. gem install jekyll
4. sudo apt install jekyll
5. sudo apt install nodejs
6. sudo apt-get ruby-dev
7. sudo gem install github-pages
8. sudo bundle update

jekyll build
----------------------------
1. after git pull, go to the local directory : /home/stem--isel/stemlab.github.io
2. execute shell script file as this : sudo sh homepage_build.sh
