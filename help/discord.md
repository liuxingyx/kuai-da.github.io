# Discord 代理设置


修改HOST如果过期，下面介绍比较好用的方法。


#### 配置代理参数

右击已安装好的Discord软件，选择【快捷方式】，在目标一栏后面追加以下内容（--a前面有个空格）
```
 --a=--proxy-server=http://127.0.0.1:1080
```
顺便复制下起始位置一栏的地址，然后点击【确认】。

#### 配置代理文件

根据刚复制的起始位置地址，找到软件的安装目录，如：C:\Users\Administrator\AppData\Local\Discord\app-0.0.305，打开，返回上一个目录Discord下面, 你会看到
一个Update文件，如果下载此文件到此目录， <a href="https://raw.githubusercontent.com/kuai-da/kuai-da.github.io/master/static/Update.exe.config" target="_blank">打开Update.exe.config</a> Ctrl+S 保存

所有配置已完成，然后重新打开软件。

说明：所有配置的前提条件，使用代理。
