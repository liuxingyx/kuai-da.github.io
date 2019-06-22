# Linux使用教程


### GUI客户端

####  下载


下载地址： <a href="https://github.com/shadowsocks/shadowsocks-qt5/releases/download/v3.0.1/Shadowsocks-Qt5-3.0.1-x86_64.AppImage" target="_blank">点击下载</a>


#### 运行

右击下载的文件，选择【属性】->【权限】，所有的访问都选择【读写】，并且勾选【允许作为程序执行文件】，然后右击选择【运行】。



#### 添加账号

购买的账号页面右侧二维码下面有个复制链接，复制后，点击客户端软件的【连接】->【添加】->【url】 粘贴后点击ok,

配置名称随便填写，建议写节点的中文备注，如果：日本、洛杉矶登陆。

本地地址：127.0.0.1  

端口: 1085

本地服务器类型；sockes5

然后点击 ok，然后在右击你添加的这条数据，选择【连接】


#### 浏览器配置

这里以火狐浏览器为例，

打开火狐浏览器，点击浏览器右上方【三】这个样子的菜单，选择【首选项】

网络设置【设置】

选择【手动代理配置】，socks5主机填写；127.0.0.1   ，端口填写；1085  ，选择socks_v5 ,点击确定。

试试可以打开谷歌了吗。

以上代理是全剧代理，所有的网站都会走代理，想国内的baidu之类的网站也会走代理，

还有一种pac模式【推荐】，pac模式意思是近需要代理的网站走代理，国内的网站不走代理。


#### pac生成

安装pip
```
apt-get install python-pip
```

安装GenPAC
```
sudo pip install genpac
pip install --upgrade genpac
```
生产pac文件
```
genpac --pac-proxy "SOCKS5 127.0.0.1:1085" --gfwlist-proxy="SOCKS5 127.0.0.1:1085" --gfwlist-url=https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt --output="autoproxy.pac"
```
完成后，当前目录会看到一个 autoproxy.pac的文件，

然后还是在火狐浏览器代理设置那里，选择【自动代理配置的url(pac)】,粘贴生产文件的目录地址，点击【重新载入】。

例子；ubuntu系统文件地址的为： file:///xxx/xxx/autoproxy.pac  (xxx换成你的文件所在目录哦)



如果不行，请下载个远程协助软件 <a href="https://www.teamviewer.cn/cn/download" target="_blank">teamviewer</a>, 安装后，把id和密码发给我，我远程帮你看看





