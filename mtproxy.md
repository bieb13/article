## 一键搭建tg mtproxy
>前提:你得有一个vps

某人白嫖谷歌云，因为自己也是新手，没怎么用gcp只是开了几台小🐔给朋友玩玩，现在只剩两个月的时间了，送的体验金还有二百多刀，用来折腾一下，顺便学习一下。

> 我的vps是utuban系统，且装了宝塔面板

所以操作非常简单，连接到SSH后

一键代码输入

```markdown
mkdir /home/mtproxy && cd /home/mtproxy
curl -s -o mtproxy.sh https://raw.githubusercontent.com/ellermister/mtproxy/master/mtproxy.sh && chmod +x mtproxy.sh && bash mtproxy.sh
```

- 对了因为我装了宝塔面板，所以默认的`443`和`8888`端口已经被占用，所以要记得在宝塔-安全里 新增两个端口放行，备注方便自己记忆就行(端口一会儿会用到)
- 根据提示选择输入指定 端口(刚刚放行的端口)
- 如果没有特殊需求，一路默认下去就行
- 当当当！成功安装并且运行（下图是脚本作者图例）
![](https://i2.wp.com/b2.bietalk.com/img/5b3fd65e-9ecd-4060-a0fe-dbf749c53b20.png)

    
- 如果想卸载也非常简单 直接rm 该文件的所在目录即可
- 我输出后的链接，发现无法直接使用的，然后发现去tg代理里手动添加即可，把主机IP地址，端口填写进去，MTProxy Secrect填进去。成功保存，连接，分享。完美

![](https://i2.wp.com/b2.bietalk.com/img/2811b44d-6508-4f83-add5-fc47b9a355a8.png)
- 🥰

*转载请附带原文链接 谢谢*