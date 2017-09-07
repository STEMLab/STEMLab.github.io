Spatio-Temporal Databases Labaratory home page


ruby version is now managed by rbenv. So after clone this, if environment doesn't use rbenv, then do this.

-------------------------------------
cd $HOME
sudo apt-get remove ruby
sudo apt-get update 
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev

git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 2.3.1
rbenv global 2.3.1
ruby -v
-----------------------------------
Reference for upper steps : 
https://stackoverflow.com/questions/37720892/you-dont-have-write-permissions-for-the-var-lib-gems-2-3-0-directory

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
9. sudo bundle exec jekyll build -d '/home/stem--isel/server/web' --baseurl '/web'
  #warnning : if you build at destination, the content of dest will be removed all and newly put build result.

  
