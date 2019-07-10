# CentOS 7 Server Configurations

Create first user w/ ssh:

```sh
adduser johnpyp
passwd johnpyp
gpasswd -a johnpyp wheel
cp -r ~/.ssh /home/johnpyp
chown -R johnpyp:johnpyp /home/johnpyp/.ssh
```
