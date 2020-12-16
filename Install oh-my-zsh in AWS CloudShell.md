## Install oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
echo 'exec /bin/zsh' >> ~/.bash_profile
sed -i "/^plugins=/c\plugins=(git aws)" ~/.zshrc
source ~/.bash_profile
exit
```
