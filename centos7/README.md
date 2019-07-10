# CentOS 7 Server Configurations

Create first user w/ ssh:

```sh
adduser johnpyp
passwd johnpyp
gpasswd -a johnpyp wheel
cp -r ~/.ssh /home/johnpyp
chown -R johnpyp:johnpyp /home/johnpyp/.ssh
su - johnpyp
```

ZSH stuff:

```
sudo yum install -y zsh git vim
sudo sh -c "curl -sfL git.io/antibody | sh -s - -b /usr/local/bin"
chsh -s /bin/zsh
curl https://raw.githubusercontent.com/johnpyp/server-recipes/master/centos7/zsh/.zshrc -o ~/.zshrc
curl https://raw.githubusercontent.com/johnpyp/server-recipes/master/centos7/zsh/.zplugins.txt -o ~/.zplugins.txt
antibody bundle < ~/.zsh_plugins.txt > ~/.zsh_plugins.sh
```
