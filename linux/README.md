# Linux使用教程

<!-- > An awesome project. -->

#### GUI客户端

#####  Fedora


The Copr builds RPMs for latest Fedora. You can enable the repo via dnf:

```
sudo dnf copr enable librehat/shadowsocks
sudo dnf update
sudo dnf install shadowsocks-qt5
```
You may need to install a dnf plugin via the command below, before you can enable copr repo using dnf.

sudo dnf install dnf-plugins-core
If your distribution doesn't have dnf, you can download the corresponding yum repo from Copr and put it under /etc/yum.repos.d/, then install shadowsocks-qt5 via yum:

```
sudo yum update
sudo yum install shadowsocks-qt5
```


##### Debian

<a href="https://github.com/debiancn/repo" target="_blank">Debian CN</a> 



##### Arch

<a href="https://www.archlinux.org/packages/community/x86_64/shadowsocks-qt5/" target="_blank">Community</a> 



##### Gentoo

<a href="https://github.com/microcai/gentoo-zh" target="_blank">gentoo-zh</a> maintained by microcai



#### 命令行客户端

```
pip install shadowsocks
apt-get install shadowsocks-libev
cpan Net::Shadowsocks
```





