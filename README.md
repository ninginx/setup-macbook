# Set up MacBook


```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

# brew install git

# setup nodenv & nodejs
brew install anyenv
# not working
echo 'eval "$(anyenv init -)"' >> ~/.bash_profile
exec $SHELL -l
anyenv install nodenv
exec $SHELL -l

mkdir -p $(anyenv root)/plugins
git clone https://github.com/znz/anyenv-update.git $(anyenv root)/plugins/anyenv-update
mkdir -p "$(nodenv root)"/plugins

```